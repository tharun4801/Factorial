# Factorial
#global variables
fact=1
def factorial(n):
    global fact
    fact=1
    for i in range(1,n+1):
        fact*=i
    return fact
num=int(input("enter a number"))
if num<0:
    print("cannot derive factorial for negative number")
else:
    factorial(num)
    print(f"Factorial of {num} is",fact)
OUTPUT:
enter a number 4
Factorial of 4 is 24

#while function
n=int(input("enter a number:"))
fact=1
i=1
while i<=n:
    fact*=i
    i+=1
print(f"Factorial of {n} is",fact)
OUTPUT:
enter a number 4
Factorial of 4 is 24

#math function
import math
n=int(input("enter a number:"))
print(f"Factorial of {n} is {math.factorial(n)}")
OUTPUT:
enter a number 4
Factorial of 4 is 24

# recursive function
def factorial(n):
    if n==0 or n==1:
        return 1
    return n*factorial(n-1)
num=int(input("enter a number:"))
value=factorial(num)
print(value)
OUTPUT:
enter a number: 5
120
