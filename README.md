# CALC
import math
user_name = str(input("Enter your name pls: ")).strip( ).title( )
def msg(name):
    print("="*45)
    print(f"         GOOD DAY FUTURE PROGRAMMER\n{user_name.center(45)}")
    print("="*45)
msg(user_name)  
print("     Hello world \n let's  do some math")
print("="*45)
choice = "AVAILABLE OPTIONS"
text = choice.center(45)
#calculator
while True:
        print(text)
        print("1.Addition")
        print("2.Subtraction")
        print("3.Multiplication")
        print("4.Division")
        print("5.Exponent")
        print("6.Squareroot")
        print("7.Exit")
        
        try:
            choice = int(input("Choose an option: 1-7 : "))
        except ValueError:
            print("INVALID INPUT,PLEASE ENTER A NUMBER BETWEEN 1-7")
            continue
        if choice < 1 or choice > 7:
            print("INVALID INPUT,PLEASE ENTER A NUMBER BETWEEN 1-7")
            continue
        
        if choice == 7:
            print(f"GOODBYE,{user_name}")
            break
        elif choice == 1:
            try:
                num_1 = float(input("Enter a number: "))
                num_2 = float(input("Enter another number: "))
                print("RESULT:", num_1 + num_2)
            except ValueError:
                print("INVALID INPUT,PLEASE ENTER NUMBERS ONLY")
        elif choice == 2:
            try:
                num_1 = float(input("Enter a number: "))
                num_2 = float(input("Enter another number: "))
                print("RESULT:", num_1 - num_2) 
            except ValueError:
                print("INVALID INPUT,PLEASE ENTER NUMBERS ONLY")
        elif choice == 3:
            try:
                num_1 = float(input("Enter a number: "))
                num_2 = float   (input("Enter another number: "))
                print("RESULT:", num_1 * num_2)
            except ValueError:
                print("INVALID INPUT,PLEASE ENTER NUMBERS ONLY") 
        elif choice == 4:
            try:
                num_1 = float(input("Enter a number: "))
                num_2 = float(input("Enter another number: "))
                print("RESULT:", num_1 / num_2)
            except ValueError:
                print("INVALID INPUT,PLEASE ENTER NUMBERS ONLY") 
            except ZeroDivisionError:
                print("YOU KNOW YOU CANNOT DO THAT RIGHT? \nDIVIDING BY ZERO IS NOT ALLOWED \n") 
        elif choice == 5:
            try:
                num_1 = float(input("Enter the base number: "))
                num_2 = float(input("Enter the exponent number: "))
                print("RESULT:", num_1 ** num_2)
            except ValueError:
                print("INVALID INPUT,PLEASE ENTER NUMBERS ONLY")
        elif choice == 6:
            try:
                num_1 = float(input("Enter a number: "))
                if num_1 < 0:
                    print("CANNOT COMPUTE SQUAREROOT OF A NEGATIVE NUMBER,PLEASE ENTER A VALID NUMBER \n")
                else:
                    print("RESULT:", num_1 ** 0.5)
            except ValueError:
                print("INVALID INPUT,PLEASE ENTER NUMBERS ONLY \n")
    
    
    
    
    
