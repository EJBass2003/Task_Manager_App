# Task_Manager_App
This task manager app allows users to manage tasks with the ability to add, view, mark as complete, and reset tasks. It uses SharedPreferences for persistent storage to save and retrieve the tasks across app sessions.

Screen Breakdown:

1. Main Screen (Task List):
  * Purpose: Displays a list of tasks that the user has added.

  * Components:
    - A RecyclerView or ListView that displays tasks.
    - Each task has a checkbox to mark it as complete or incomplete.
    - A button to navigate to the "Add Task" screen.

2. Add Task Screen:
  * Purpose: Allows the user to add a new task to the list.

  * Components:
    - An EditText to enter the task name.
    - A "Save" button that saves the task to SharedPreferences.
    - Once saved, it redirects the user back to the Task List screen.

3. Task Detail Screen:
  * Purpose: View the details of a specific task.

  * Components:
    - A TextView displaying the task name.
    - A checkbox to mark the task as completed.
    - A button to delete the task from the list.
    - This screen uses Intent to pass data from the Task List screen.

4. Settings Screen:
  * Purpose: Allows the user to reset all tasks and customize aesthetics.

  * Components:
    - A button to reset all tasks, clearing them from SharedPreferences.
    - An option to toggle between Light Theme and Dark Theme
    - An option to toggle the text size between small, medium, and large
   
