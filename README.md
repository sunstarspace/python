# **Python basics**


## Check if the year is leap:

```python
# User input
year = int(input("Enter a year, please: "))

if year % 4 == 0:
    if year % 100 == 0:
        if year % 400 == 0:
            print(f'Leap year!')
        else:
            print(f'Not a leap year!')
    else:
        print(f'Leap year!')
else:
    print(f'Not a leap year!')
```

<br />

## BMI calculator:

```python
# User input
height = float(input("Please, enter your height (in m): "))
weight = float(input("Please, enter your weight (in kg): "))

bmi = round(weight / height ** 2)

print("BMI is approximatelly: " + str(int(bmi)))
print(type(bmi))

if bmi < 18.5:
    print(f'BMI is {bmi} - underweight')
elif bmi < 25:
    print(f'BMI is {bmi} - normal weight')
elif bmi < 30:
    print(f'BMI is {bmi} - overweight')
elif bmi < 35:
    print(f'BMI is {bmi} - obese')
else:
    print(f'BMI is {bmi} - you should start sporting')
```