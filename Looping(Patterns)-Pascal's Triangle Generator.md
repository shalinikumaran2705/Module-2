# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

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

## 🧪 Program
```python
n = int(input("Enter the number of rows: "))
for i in range(n):
    print(" " * (n - i), end="")
    for j in range(i + 1):
        value = 1
        for k in range(j):
            value = value * (i - k) // (k + 1)
        print(value, end=" ")
    print()
```
## Sample Output

<img width="482" height="212" alt="image" src="https://github.com/user-attachments/assets/518df92a-153b-4956-a361-6aa6bccf88ea" />

## Result
Thus, the Python program was successfully executed to generate Pascal's Triangle for the given number of rows.

