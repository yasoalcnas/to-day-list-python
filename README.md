# to-day-list-python
print("__________________________________")
print("------------to do list app--------")
print("----------------------------------")
print("                              ")
print("add task = 1:-")
print("show task = 2:-")
print("delete task = 3:-")
print("exit = 4:-")
print("                              ")

# define tasks dictionary before using it
stordg_tasks = {
    1: "",
    2: "",
    3: "",
    4: "",
    5: "",
}

# loop to keep the program running
while True:
  # ask user for a task number
  numper_request_input = input("Enter number of your request (1-4): ")

  #system of choosing the order
  def Choose_the_order():
    if numper_request_input == "1":
      add_task()
    elif numper_request_input == "2":
      show_task()
    elif numper_request_input == "3":
      delete_task()
    elif numper_request_input == "4":
      exit()
    pass

  #function to add task
  def add_task():
    task = input("Enter your task: ")
    numper_task_input = input("Enter add number of your task (1-5): ")
    if numper_task_input == "1":
      stordg_tasks[1] = task
    elif numper_task_input == "2":
      stordg_tasks[2] = task
    elif numper_task_input == "3":
      stordg_tasks[3] = task
    elif numper_task_input == "4":
      stordg_tasks[4] = task
    elif numper_task_input == "5":
      stordg_tasks[5] = task
    pass

  #function to show task
  def show_task():
    numper_task_show = input("Enter add number of your task (1-5): ")
    if numper_task_show == "1":
      print(stordg_tasks[1])
    elif numper_task_show == "2":
      print(stordg_tasks[2])
    elif numper_task_show == "3":
      print(stordg_tasks[3])
    elif numper_task_show == "4":
      print(stordg_tasks[4])
    elif numper_task_show == "5":
      print(stordg_tasks[5])
    pass

  #function to delete task
  def delete_task():
    numper_task_delete = input("Enter add number of your task (1-5): ")
    if numper_task_delete == "1":
      stordg_tasks[1] = ""
    elif numper_task_delete == "2":
      stordg_tasks[2] = ""
    elif numper_task_delete == "3":
      stordg_tasks[3] = ""
    elif numper_task_delete == "4":
      stordg_tasks[4] = ""
    elif numper_task_delete == "5":
      stordg_tasks[5] = ""
    pass

  #function to exit
  def exit():
    quit()
    pass

  Choose_the_order()
