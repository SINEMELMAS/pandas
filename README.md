# pandas
# python-
import numpy as np
import pandas as pd

print("Program is working. If you want stop it just enter stop!")
numbers = []
squares = []
while True:
    number = input("enter a number: ")
    if number == "stop":
        print("program stopped.")
        dataframe=pd.DataFrame({'number': numbers,'square': squares})
        print(dataframe)
        break   
    try:
        sqr=float(number)**2
        numbers.append(float(number))
        squares.append(sqr)
        print(f"sqr of the number= {sqr}") 
        
    except ValueError:
        print("Invalid input. Please enter a valid number.")
            

