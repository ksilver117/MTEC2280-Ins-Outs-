
import serial
ser = serial.Serial("/dev/cu.usbmodemfa131",9600)

print ("Make sure to start with a space then capital letter before you put your answer")
state = 0

while(True):
    if (state == 0):
        Round1 = input("Name some things that little kids hate to do")
        if (Round1 == " Go to bed" ):

            message = "correct" + "\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 1

        elif (Round1 == " Take a bath"):

            message = "correct" + "\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 1

        elif (Round1 == " Brush their teeth") :

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 1

        elif (Round1 == " Clean their room"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 1

        elif (Round1 == " Eat vegetables"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 1

        elif (Round1 == " Pick up toys"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 1

        elif (Round1 == " Go to dentist"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 1

        elif (Round1 == " Take medecine"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 1


        else :
            message = "wrong"+"\n"
            message = message.encode()
            ser.write(message)
            print ("wrong answer")
            state = 0

    if(state == 1):
        Round2 = input("Give me another term for mother")
        if (Round2 == " Mom"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 2
        elif (Round2 == " Mama"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 2
        elif (Round2 == " Mommy"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 2
        elif (Round2 == " Ma"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 2
        else  :
            message ="wrong"+"\n"
            message = message.encode()
            ser.write(message)
            print ("wrong answer")
            state = 1

    if (state == 2):
        Round3 = input("Name a white animal")

        if (Round3 == " Polar bear"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 3

        elif (Round3 == " Rabbit"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 3

        elif (Round3 == " Cat"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 3

        elif (Round3 == " Horse"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 3

        elif (Round3 == " Seal"):

            message = "correct"+"\n"
            message = message.encode()
            ser.write(message)
            print ("correct")
            state = 3

        else  :
            message = "wrong"+"\n"
            message = message.encode()
            ser.write(message)
            print ("wrong answer")
            state = 2

    if (state == 3):
        GameOver = input("Thanks for playing!")

ser.close()               
