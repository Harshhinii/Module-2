## PYTHON PROGRAMMING MODULE 2
## NAME: HARSHINI R
## REGISTER NUMBER: 212223220033
## Ex 01: Built-in Functions -Binary Conversion Using Built-in Functions in Python

##  Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

##  Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

##  Program
```
a = 16
print(bin(a))
```

## Output

<img width="1181" height="267" alt="604170897-4516c7f0-846e-41ac-8aac-8309dcca1749" src="https://github.com/user-attachments/assets/9e1c587e-d7c9-4fa4-a963-c4207c5a774d" />


## Result
The program successfully converts the number 16 into its binary representation and prints it.

## Ex 02:Functions in Python: Modulo Calculator

##  Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

##  Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

##  Program
```
def result(a, b):
    return a % b

a = int(input())
b = int(input())
print("The result of the modulo operation is:", result(a, b))
```

## Output
<img width="1181" height="278" alt="604171569-0ee91fae-6ce2-43fa-aa43-89731c755458" src="https://github.com/user-attachments/assets/432ad164-0e21-434e-8952-ef290a654a34" />



## Result
The program successfully defines a function that computes the modulo of two numbers and returns the result.

## Ex 03: Lambda Function in Python: Addition of Two Numbers

##  Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

##  Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

##  Program
```
i=int(input())
j=int(input())
z=int(input())
f = lambda a, b,c: a+b+c
print(f(i, j,z))
```
## Output

<img width="535" height="415" alt="604172189-fe784b66-9889-4da8-827b-532b50d6a790" src="https://github.com/user-attachments/assets/84734d39-d81a-454f-b36e-2c3b4e13f798" />


## Result
The program successfully defines a lambda function that computes the sum of two numbers and prints the result.

## Ex 04: Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

##  Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

##  Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

##  Program
```
rows = int(input())
coef = 1

for i in range(1, rows+1):
    for space in range(1, rows-i+1):
        print(" ",end="")
    for j in range(0, i):
        if j==0 or i==0:
            coef = 1
        else:
            coef = coef * (i - j)//j
        print(coef, end = " ")
    print()
```

## Sample Output

<img width="666" height="752" alt="604172886-0b85aa27-e71a-49fd-8f8d-4e5e92a703ae" src="https://github.com/user-attachments/assets/95887930-4177-47db-b56c-56f5f1632b7c" />


## Result
The program successfully generates Pascal's Triangle with the specified number of rows, using the appropriate formula for combination values

## Ex 05: Loops in Python: Palindrome Number Checker

##  Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

##  Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

##  Program
```
num = int(input())
temp = num
rev = 0

while temp > 0:
    rev = (10 * rev) + temp % 10
    temp = temp // 10

if rev == num:
    print(f"{num} is a palindrome.")
else:
    print(f"{num} is not a palindrome.")
```
## Output
<img width="1031" height="275" alt="604173456-6f3c15b9-c135-4745-b3d0-b3f67e3ad045" src="https://github.com/user-attachments/assets/934d50d4-574e-4243-adf6-1caf4edfb052" />

## Result
The program successfully checks if a given number is a palindrome by reversing its digits and comparing it to the original number.

