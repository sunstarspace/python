<br />

# **Python basics**

<br />

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