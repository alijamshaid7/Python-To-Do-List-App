**# To Do App in PYTHON**



def task():

&#x20;   tasks = \[]  # Initialize an empty list to store tasks

&#x20;   print("----WELCOME TO THE TASK MANAGEMENT APP----")

&#x20;   total\_task = int(input("Enter how many tasks you want to add = "))

&#x20;   for i in range(1, total\_task + 1):

&#x20;       task\_name = input(f"Enter task {i} = ")

&#x20;       tasks.append(task\_name)

&#x20;   print(f"Today's tasks are\\n{tasks}")

&#x20;   

&#x20;   while True:

&#x20;       try:

&#x20;           operation = int(input("Enter \\n1-Add\\n2-Update\\n3-Delete\\n4-View\\n5-Exit/Stop\\n"))

&#x20;           if operation == 1:

&#x20;               add = input("Enter task you want to add = ")

&#x20;               tasks.append(add)

&#x20;               print(f"Task '{add}' has been successfully added.")

&#x20;           elif operation == 2:

&#x20;               updated\_val = input("Enter the task name you want to update = ")

&#x20;               if updated\_val in tasks:

&#x20;                   up = input("Enter new task = ")

&#x20;                   ind = tasks.index(updated\_val)

&#x20;                   tasks\[ind] = up

&#x20;                   print(f"Updated task '{updated\_val}' to '{up}'.")

&#x20;               else:

&#x20;                   print("Task not found.")

&#x20;           elif operation == 3:

&#x20;               del\_val = input("Which task you want to delete = ")

&#x20;               if del\_val in tasks:

&#x20;                   ind = tasks.index(del\_val)

&#x20;                   del tasks\[ind]

&#x20;                   print(f"Task '{del\_val}' has been deleted.")

&#x20;               else:

&#x20;                   print("Task not found.")

&#x20;           elif operation == 4:

&#x20;               print(f"Total tasks = {tasks}")

&#x20;           elif operation == 5:

&#x20;               print("Closing the program....")

&#x20;               break

&#x20;           else:

&#x20;               print("Invalid Input. Please enter a number from 1 to 5.")

&#x20;       except ValueError:

&#x20;           print("Invalid Input. Please enter a valid number.")



task()



&#x20;

