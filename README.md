# **Python basics**


## Check leap year:

```python
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

## BMI calculator:

```python
height = float(input("enter your height in m: "))
weight = float(input("enter your weight in kg: "))

bmi = round(weight / height ** 2)
# or bmi = weight_as_int / (height_as_float * height_as_float)

print("Your BMI is approximatelly: " + str(int(bmi)))
print(type(bmi))

if bmi < 18.5:
    print(f'Your BMI is {bmi} - underweight')
elif bmi < 25:
    print(f'Your BMI is {bmi} - normal weight')
elif bmi < 30:
    print(f'Your BMI is {bmi} - overweight')
elif bmi < 35:
    print(f'Your BMI is {bmi} - obese')
else:
    print(f'Your BMI is {bmi} - you should start sporting')
```