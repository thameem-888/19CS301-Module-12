# 19CS301-Module-12

EX: 12.1   Stack using linked list (Display, Peek and Pop)


### AIM: 

To insert a few elements into a stack and check whether the stack is full or not.

### ALGORITHM:
Step 1: Define a class Stack with methods __init__, is_full, push, and display.

Step 2: In __init__, initialize the stack list and define the maximum size.

Step 3: In is_full, check whether the number of elements has reached the maximum size.

Step 4: In push, insert elements into the stack if it's not full.

Step 5: In display, print the current elements of the stack.

Step 6: Create a Stack object and push a few elements.

Step 7: Check and display whether the stack is full.



### PROGRAM:
```
class Stack:
    def __init__(self, max_size):
        self.stack = []
        self.max_size = max_size

    def push(self, item):
        if not self.is_full():
            self.stack.append(item)

    def is_full(self):
        return len(self.stack) == self.max_size


# Create a stack with a maximum size of 5
s = Stack(5)

# Insert a few elements (less than 5)
s.push(10)
s.push(20)
s.push(30)

# Check if the stack is full and print result
if s.is_full():
    print("Stack is full")
else:
    print("Stack is not full")

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/32e93e2a-b0a8-4eaf-b4de-f42c6ab83c61)


### RESULT: 

Thus, the program has been successfully executed.

EXP.No: 12.2 Stack using linked list (Push and all operations)

### AIM: 

To get 3 inputs from the user, insert them into a stack, and print each element along with its respective index value.

###ALGORITHM:
Step 1: Initialize an empty list to represent the stack.

Step 2: Use a loop to get 3 inputs from the user.

Step 3: Append each input into the stack.

Step 4: Use a loop with enumerate() to print each element with its index value.

### PROGRAM:
```
stack = []
stack.append(input("Insert the first element:"))
stack.append(input("\nInsert the second element:"))
stack.append(input("\nInsert the third element:"))

print('\nInitial stack: ' + str(stack))

for i in range(len(stack)):
    print(i,end=" ")
    print(stack[i])


```
###OUTPUT:


![image](https://github.com/user-attachments/assets/06e3ab0a-0dcf-4488-88a5-34a56dec25a5)




###RESULT: 

The program successfully accepts 3 user inputs, inserts them into a stack, and prints each element along with its corresponding index value.


EX: 12.3  Queue using linked list (Display, Peek and Pop)

### AIM: 

To list all candidates who appeared for the interview and find the slot numbers of both candidates named "Ram".

### ALGORITHM:

Step 1: Create a list of candidate names representing their slot order.

Step 2: Traverse the list using a loop.

Step 3: Compare each name (case-insensitive) to "Ram".

Step 4: If matched, store and display the corresponding slot number(s).


### PROGRAM:


```
interview = []

interview.append("Ram")
interview.append("Priya")
interview.append("John")
interview.append("Vignesh")
interview.append("Reshma")
interview.append("Ram")
interview.append("Meeran")
interview.append("Sai kumar")
print("List of candidates appeared for the interview:")
print(interview)
print("Display the slot numbers of the candidates with same name: ")
print(interview.index("Ram",0,4))
print(interview.index("Ram",5,7))


```
### OUTPUT:

![image](https://github.com/user-attachments/assets/224c34e7-aef6-4da2-b879-31e49931b3bc)



### RESULT: 

The program displays the list of all interview candidates and correctly identifies and displays the slot numbers of both "Ram" who appeared for the interview.


EXP.No: 12.4 Queue using linked list (Enqueue and all operations)


### AIM:

To get the first 3 tasks of the day from the boss’s personal assistant and print them along with their index order.

###ALGORITHM: 

Step 1: Initialize an empty list to store tasks.

Step 2: Use a loop to get 3 task inputs from the user.

Step 3: Append each task to the list.

Step 4: Use a loop with enumerate() to print the tasks along with their index.

###PROGRAM:
```
queue= []
queue.append(input("Task_1: "))
queue.append(input("\nTask_2: "))
queue.append(input("\nTask_3: "))
print('\nTask details: ' + str(queue))

for i in range(len(queue)):
    print(i, end=" ")
    print(queue[i])

```
### OUTPUT:
 
![image](https://github.com/user-attachments/assets/93ca3293-33a4-4979-ba04-4fbb7f810513)


### RESULT: 

The program successfully accepts the first 3 tasks from the boss’s personal assistant and displays them in index order for the secretary’s reference.



EXP.No: 12.5 ASSESSMENT EXAM-SEB


### AIM:

To simulate monthly storage of rice bags in a warehouse, track sales, and determine which month's rice bags are ready for sale and which ones were recently added.


###ALGORITHM: 

Step 1: Create a list to store rice bags month-wise.

Step 2: Each month, 250 rice bags are added to the warehouse.

Step 3: Simulate sales by removing rice bags (FIFO method).

Step 4: Determine the earliest month with remaining stock (next for sale).

Step 5: Identify the most recent month of storage.



###PROGRAM:
```
queue = []

queue.append('Apr_RB4_250')
queue.append('May_RB5_250')
queue.append('June_RB6_250')

print(queue)
print("\nNext rice bag ready for sale .... Apr_RB4_250")

print("\nNew rice bag .... June_RB6_250")

```
### OUTPUT:

 ![image](https://github.com/user-attachments/assets/318861a9-402f-451c-af04-20dbd300d7a0)


### RESULT: 

The program correctly identifies the month whose rice bags are next ready for sale and the month in which rice bags were most recently added to the warehouse.







