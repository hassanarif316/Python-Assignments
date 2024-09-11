
# Favorite Numbers Program

This program allows the user to input their favorite numbers and explores various properties like even/odd classification, squares, sum, and prime status.


## Get user input
```python
name = input("Enter your name: ")
num1 = int(input("Enter your 1st favorite number: "))
num2 = int(input("Enter your 2nd favorite number: "))
num3 = int(input("Enter your 3rd favorite number: "))
```
## Store the numbers in a list
```python
listt = [num1, num2, num3]
print(f"Hello, {name}! Let's explore your favorite numbers:")

# List to store even/odd classification
eo_list = []
```
## Check each number for even/odd
```python
for i in listt:
    if i % 2 == 0:
        eo_list.append((i, "even"))
    else:
        eo_list.append((i, "odd"))
```
## Print even/odd classification for each number
```python
for num, eo in eo_list:
    print(f"The number {num} is {eo}.")

print("\n")
```
## Calculate and print the square of each number
```python
for i in listt:
    square = i ** 2
    print(f"The number {i} and its square: ({i}, {square})")
```
## Calculate the sum of the numbers
```python
add = sum(listt)
print(f"Amazing! The sum of your favorite numbers is: {add}")
```
## Check if the sum is a prime number
```python
is_prime = True
if add <= 1:
    is_prime = False

for i in range(2, add):
    if add % i == 0:
        is_prime = False
```
## Print whether the sum is prime or not
```python
if is_prime:
    print(f"Wow, {add} is a prime number!")
else:
    print(f"Oops, {add} is not a prime number.")
```

## Program Details
- **Even/Odd Classification**: Each number is checked to determine whether it is even or odd.
- **Squares**: The square of each number is calculated and printed.
- **Sum**: The sum of the three favorite numbers is calculated.
- **Prime Check**: The sum is checked to determine whether it is a prime number.
```
