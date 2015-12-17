

#include "pitches.h"
int State = 0;
int melody1 [] =
{ NOTE_C5, NOTE_E5, NOTE_G5, NOTE_C6};

int noteDurations1[] =
{4, 4, 4, 3};

int melody2[] =
{ NOTE_B5, NOTE_AS5, NOTE_A5, NOTE_GS5, NOTE_G5};

int noteDurations2[] =
{4, 4, 4, 3};

String message = "";         // a string to hold incoming data
boolean messageComplete = false;  // whether the string is complete

void setup()
{
  // initialize serial:
  Serial.begin(9600);
  // reserve 200 bytes for the inputString:
  message.reserve(200);
  pinMode(12, OUTPUT); //Buzzer
}

void loop()
{
  if (message == ("correct"))
  {
    // iterate over the notes of the melody:
    for (int thisNote = 0; thisNote < 4; thisNote++) {

      // to calculate the note duration, take one second
      // divided by the note type.
      //e.g. quarter note = 1000 / 4, eighth note = 1000/8, etc.
      int noteDuration1 = 150 / noteDurations1[thisNote];
      tone(12, melody1[thisNote], noteDuration1);

      // to distinguish the notes, set a minimum time between them.
      // the note's duration + 30% seems to work well:
      int pauseBetweenNotes = noteDuration1 * 1.30;
      delay(pauseBetweenNotes);
      // stop the tone playing:
      noTone(12);
    }

  }
  else if (message == ("wrong"))
  {
    for (int thisNote = 0; thisNote < 4; thisNote++) {

      // to calculate the note duration, take one second
      // divided by the note type.
      //e.g. quarter note = 1000 / 4, eighth note = 1000/8, etc.
      int noteDuration2 = 150 / noteDurations2[thisNote];
      tone(12, melody2[thisNote], noteDuration2);

      // to distinguish the notes, set a minimum time between them.
      // the note's duration + 30% seems to work well:
      int pauseBetweenNotes = noteDuration2 * 1.30;
      delay(pauseBetweenNotes);
      // stop the tone playing:
      noTone(12);
    }
    if (message == (""))
    {
      messageComplete = false;
    }
  }
}

void serialEvent() {
  while (Serial.available()) {
    // get the new byte:
    char inChar = (char)Serial.read();
    // add it to the inputString:
    //inputString += inChar;


    if (inChar != '\n') {
      message += inChar;
    }

    // if the incoming character is a newline, set a flag
    // so the main loop can do something about it:
    if (inChar == '\n') {
      messageComplete = true;
    }
  }
}
