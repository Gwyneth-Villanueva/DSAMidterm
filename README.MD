# HELLO 

Plain Paragraph
from fractions import Fraction
print("Advanced Calculator")
print("Choose mode:")
print("1 - Normal numbers")
print("2 - Fractions")

mode = input("Enter mode: ")

if mode == "1":
    print("Normal mode chosen")
        
    num1 = float(input("Enter first number: "))
    operator = input("Enter operator (+, -, *, /): ")
    num2 = float(input("Enter the second number: "))

    if operator == "+":
        print("Result:", num1 + num2)
    elif operator == "-":
        print("Result:", num1 - num2)
    elif operator == "*":
        print("Result:", num1 * num2)
    elif operator == "/":
        if num2 == 0:
            print("Error: Division by zero")
        else:
            print("Result:", num1 / num2)
    else:
        print("Invalid operator")

elif mode == "2":
    print("Enter fractions in the form a/b")
        
    num1 = Fraction(input("Enter first fraction: "))
    operator = input("Enter operator (+, -, *, /): ")
    num2 = Fraction(input("Enter second fraction: "))

    if operator == "+":
        print("Result:", num1 + num2)
    elif operator == "-":
        print("Result:", num1 - num2)
    elif operator == "*":
        print("Result:", num1 * num2)
    elif operator == "/":
        if num2 == 0:
            print("Error: Division by zero")
        else:
            print("Result:", num1 / num2)
    else:
        print("Invalid operator")

else:
    print("Invalid mode.")
