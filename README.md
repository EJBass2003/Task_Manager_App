# Task_Manager_App
This task manager app allows users to manage tasks with the ability to add, view, mark as complete, and reset tasks. It uses SharedPreferences for persistent storage to save and retrieve the tasks across app sessions.

Screen Breakdown:

1) **Main Screen (Task List)**
  - **Header:** “Task List” displayed prominently at the top  
  - **Scrollable Task Panel:**  
    - Vertically scrollable list showing each task (e.g. Task #1, Task #2, … Task #5)  
    - Each row is a checkbox + label combo, allowing users to mark tasks complete  
  - **Navigation Buttons** (anchored below the list):  
    - **Settings** → opens Settings screen  
    - **Add Task** → opens Add Task screen  
    - **Details** → opens Task Details screen  

2) **Add Task Screen**
  - **Toolbar:** Back-arrow + title “Add Task”  
  - **Form Fields:**  
    - **Task Name:** single-line text input  
    - **Description:** multi-line text area  
    - **Due Date:** three-part date entry (MM / DD / YYYY)  
    - **Importance:** dropdown or segmented control (e.g. High, Medium, Low)  
  - **Save Button:** commits the new task and returns to Main Screen  

3) **Task Detail Screen**
  - **Toolbar:** Back-arrow + title “Task Details”  
  - **Detail Display:**  
    - **Task Name:** large, bold label  
    - **Description:** regular text label  
    - **Due Date:** formatted date label (e.g. 1/11/1111)  
    - **Importance:** label indicating priority (e.g. High)  
  - **Action Buttons:**  
    - **Edit** → transforms fields into editable inputs (or navigates to Add-style screen pre-filled)  
    - **Delete** → triggers the Confirmation Screen  

4) **Settings Screen**
  - **Toolbar:** Back-arrow + title “Settings”  
  - **Preferences:**  
    - **Theme:** toggle or radio between Light Mode / Dark Mode  
    - **Text Color:** hex-input or color picker (e.g. #2b78e4)  
  - **Controls:**  
    - **Save** → persists aesthetic choices  
    - **Clear All Tasks** → triggers the Confirmation Screen for data reset  

5) **Confirmation Screen(s)**
  - **Modal Prompt** (or full-screen overlay):  
    - **Message:** “Do you want to delete this task?” (or “Clear all tasks?” for data reset)  
    - **Buttons:** Yes / No to confirm or cancel the action
   
