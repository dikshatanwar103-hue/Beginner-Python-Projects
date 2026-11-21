import json

tasks = []

def save_tasks():
    with open("tasks.json", "w") as file:
        json.dump(tasks, file)


while True:
    print("\n ===== TO-DO LIST =====")
    print("1 for add task")
    print("2 for view task")
    print("3 for mark task as complete")
    print("4 for remove task")
    print("5 for exit")

    choice = int(input("enter your choice: "))

    if choice == 1:
        add_task = input("enter task: ")
        tasks.append(add_task)
        save_tasks()
        print("task added succesfully!")

    elif choice == 2:
        for index, task in enumerate(tasks , start = 1):
            print(f"{index}. {task}")

    elif choice == 3:
        for index, task in enumerate(tasks, start=1):
            print(f"{index}. {task}")

        task_number = int(input("Enter task number to mark as complete: "))
        tasks[task_number - 1] += " [Completed]"
        save_tasks()
        print("task markes as complete")

    elif choice == 4:
        for index, task in enumerate(tasks, start=1):
            print(f"{index}. {task}")

        task_number = int(input("Enter task number to remove: "))
        tasks.pop(task_number-1)
        save_tasks()
        print("Task removed successfully!")

    elif choice == 5:
        print("Thanks for using To-Do List!")
        break
