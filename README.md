# 19CS301-Module-9

EX: 9.1 Matrix Operations

### AIM: 

To read a matrix using a function create_matrix() and copy the contents of matrix A to matrix B.

### ALGORITHM:
Step 1: Start

Step 2: Define a function create_matrix() to:
        
Step 3: Call create_matrix() to get matrix A

Step 4: Use copy (deep copy) to create matrix B

Step 5: Print both matrices

Step 6: Stop


### PROGRAM:
```
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M
r,c=input().split()
A=create_matrix(int(r),int(c))
print('A=',A)
B=A
print('B=',B)
```
### OUTPUT:
![image](https://github.com/user-attachments/assets/c7864f94-c5d3-4c42-889f-a9b1d15ee04b)



### RESULT: 

The program reads a matrix using a function and successfully copies it to another matrix using list slicing (deep copy).

EXP.No: 9.2 List Comprehension

### AIM: 

To write a Python class program that generates all even numbers between 200 and 300 using list comprehension and stores them in a list.


###ALGORITHM:
Step 1: Define a class EvenGenerator

Step 2: Inside the class, define a method generate_evens(start, end)
        
Step 3: Create an instance of the class

Step 4: Call the method with inputs 200 and 300

Step 5: Print the result

Step 6: End



### PROGRAM:
```
class program:
    def __init__(self,a,b,c):
        self.a=a
        self.b=b
        self.c=c
    def display(self):
        even=[i for i in range(self.a,self.c+1,self.b)]
        print(even)
a=int(input())
b=int(input())
c=int(input())
obj=program(a,b,c)
obj.display()
```
###OUTPUT:


![image](https://github.com/user-attachments/assets/a879e748-ac43-4ff1-88ea-f5b24a88e0d1)




###RESULT: 

The class-based program successfully generates all even numbers between 200 and 300 using list comprehension.


EX: 9.3 Advanced Processing

### AIM: 

To subtract two matrices using list comprehension in Python.

### ALGORITHM:

Step 1: Start

Step 2: Read number of rows and columns

Step 3: Read elements of matrix A

Step 4: Read elements of matrix B

Step 5: Use list comprehension to subtract B from A

Step 6: Print matrix A, B, and the result

Step 7: Stop

### PROGRAM:


```from abc import ABC
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M

r,c=input().split()
r=int(r)
c=int(c)
A=create_matrix(r,c)
B=create_matrix(r,c) 
print(A)
print(B)
T = [[A[i][j] - B[i][j]for j in range(len(A[0]))] for i in range(len(A))]
print(T)

```
### OUTPUT:

![image](https://github.com/user-attachments/assets/aa3fd2b9-e479-49b5-bcfa-f4b338406e92)



### RESULT: 

The program correctly reads two matrices from input, subtracts them using list comprehension, and prints the result as required.

EXP.No: 9.4     Sorting


### AIM:

To implement selection sort using a class with functions to create, sort, and print a list.

###ALGORITHM: 

Step 1: Start

Step 2: Create a class named Numbers

Step 3: Define method create_list() to take list input from the user

Step 4: Define method sorting() to perform selection sort:

Step 5: Define method print_list() to print list elements

Step 6: Create an object and call the methods as required

Step 7: Stop

###PROGRAM:
```
class Numbers:
    def __init__(self, N=0):
        self.N = int(input())
    def create_list(self):
        self.L = []
        for i in range(self.N):
            x=int(input())
            self.L.append(x)
    def sorting(self):
        for ind in range(self.N):
            min_index = ind
            for j in range(ind + 1, self.N):
                if self.L[j] < self.L[min_index]:
                    min_index = j
            (self.L[ind], self.L[min_index]) = (self.L[min_index], self.L[ind])
    def print_List(self):
        for i in range(self.N):
            print(self.L[i])
```
### OUTPUT:
 
![image](https://github.com/user-attachments/assets/25b7eec0-e269-4874-8823-2ff4d4287ded)

### RESULT: 

The class-based program successfully performs selection sort on a list created by user input and displays the list before and after sorting.


EXP.No: 9.5     ASSESSMENT EXAM


### AIM:

To store a scalar multiple of a set of numbers in a list using list comprehension in Python.

###ALGORITHM: 

Step 1: Start

Step 2: Read the scalar value

Step 3: Read the number of elements

Step 4: Read the elements into a list

Step 5: Use list comprehension to multiply each element by the scalar

Step 6: Print the original list and the result list

Step 7: Stop

###PROGRAM:
```
a=int(input())
b=int(input())
l=[]
for i in range(a):
    x=float(input())
    l.append(x)
print(l)
z=[x*b for x in l ]
print(z)
```
### OUTPUT:
 
![image](https://github.com/user-attachments/assets/05fde142-4097-4408-9587-9b193fecfc4c)

 

### RESULT: 

Thus, the program has been successfully executed

