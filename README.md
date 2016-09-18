# hackerranksolution

### Reading Raw Input ###

import sys

name=input()

print (name)

### Python If-Else ###

import sys

N = int(input().strip())

if N % 2 != 0:
    print ("Weird")
elif 2<=N<=5:
    print ("Not Weird")
elif 6<=N<=20:
    print ("Weird")
elif N>20:
    print ("Not Weird")


### Arithmetic Operators ###

a=int(input())
b=int(input())
print (a+b)
print (a-b)
print (a*b)


### Python: Division ###

import sys

a=int(input())
b=int(input())

print (a//b)
print (a/b)

<<<<Loops>>>>

N=int(input())

i=list(range(0,21))

for n in i:
    if n<N:
        print(n**2)

### Write a function ###

def is_leap(year):
    if year % 400 == 0:
        return True
    if year % 100 == 0:
        return False
    if year % 4 == 0:
        return True
    return False

year = int(input())
print(is_leap(year))

### Print Function ###
print(*range(1, int(input()) + 1), sep="")  

### Lists ###
T = int(input())

L = []

for t in range(T):
    args = input().split(" ")
    if args[0] == "append":
        L.append(int(args[1]))
    elif args[0] == "insert":
        L.insert(int(args[1]), int(args[2]))
    elif args[0] == "remove":
        L.remove(int(args[1]))
    elif args[0] == "pop":
        L.pop()
    elif args[0] == "sort":
        L.sort()
    elif args[0] == "reverse":
        L.reverse()
    elif args[0] == "print":
        print (L)

### List Comprehensions ###
import sys

x = int(input())
y = int(input())
z = int(input())
n = int(input())

list=[[xx,yy,zz] for xx in range(x+1) for yy in range(y+1) for zz in range(z+1) if xx+yy+zz !=n]

print (list)

### Find the Second Largest Number ###

import sys

N = int(input())
if N >= 2 and N <= 10:
    A_s = input()
    A = set([int(x) for x in A_s.split(" ")])
    if all( n >= -100 and n <= 100 for n in A):
        A.remove(max(A))
    print (max(A))
    
    
### Nested Lists ###
