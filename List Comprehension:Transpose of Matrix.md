# 🧮 List Comprehension:Transpose of Matrix 

## 🎯 AIM:
To write a Python program to compute the **transpose** of a matrix using **list comprehension**.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` to represent the number of rows and columns of the matrix.
3. Get the values of `r` and `c` from the user.
4. Define a function `create(r, c)` to create the matrix by reading the elements from the user.
5. Use **list comprehension** to calculate the transpose of the matrix.
6. Print the transposed matrix.
7. **Stop**

---


## 💻 PROGRAM:
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
r=int(r)
c=int(c)
A=create_matrix(r,c)
B=create_matrix(r,c)
print(A)
print(B)
T = [[A[i][j] + B[i][j] for j in range(len(A[0]))] for i in range(len(A))]
print(T)
```

## OUTPUT:
<img width="956" height="827" alt="image" src="https://github.com/user-attachments/assets/e56900d5-175e-4d7f-9b3c-d66179b3ce17" />

## RESULT:
Thus,the program is executed successfully

