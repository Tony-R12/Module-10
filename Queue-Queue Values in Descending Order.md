# Queue-Queue Values in Descending Order Using Python 🧮

This Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

## 🎯 Aim

To write a Python program to:
- Accept user inputs into a list (queue)
- Remove the first two elements (simulating dequeue)
- Display the remaining values in **descending order**

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` to determine how many elements will be added.
3. Loop `n` times:
   - Read an input value.
   - Append it to the list `q`.
4. Remove the first element using `pop(0)`.
5. Remove the second element using `pop(0)` again.
6. Sort the list in descending order.
7. Print the updated list.

## 🧪 Program: 
```\import queue  
q = queue.Queue() 
for i in range(5):
    q.put(float(input()))  

n =  q.qsize()  
for i in range(n):  
    x = q.get()  
    for j in range(n-1):  
        y = q.get()  
        if x < y :  
            q.put(y)  
        else:  
            q.put(x)  
            x = y     
    q.put(x)  
while (q.empty() == False):   
    print(q.queue[0], end = " ")    
    q.get()
```

### Output:
<img width="755" height="395" alt="image" src="https://github.com/user-attachments/assets/e6cc1754-37cc-454d-bdc4-a8660d59614d" />


## Result:
Thus,the program is successfully created.
