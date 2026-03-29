## Manual Test Pack – Task Board (SoftUni Demo Project)  
App/Site: https://replit.com/@martinpetrov727/TaskBoardV01-2  
Date: 23.03.2026  
Tester: Martin Petrov  

---

## Scope
Testing the Task Board application based on the provided Software Requirements Specification (SRS).

---

## Test Cases

### TC-001 - Display welcome message on home page
Preconditions:
- User is on the home page

Steps:
1. Open the home page

Expected Result:
- Welcome message is displayed containing the text "Welcome"


### TC-002 - Verify side menu options
Preconditions:
- User is on the home page

Steps:
1. Observe the side menu

Expected Result:
- Side menu contains: Home, Task Board, Create, Search (in correct order)


### TC-003 - Display total number of tasks
Preconditions:
- User is on the home page

Steps:
1. Observe the task summary section

Expected Result:
- Total number of tasks is displayed correctly


### TC-004 - Task summary organization
Preconditions:
- User is on the home page

Steps:
1. Observe the task summary section

Expected Result:
- Tasks are grouped by boards


### TC-005 - Quick access buttons visibility
Preconditions:
- User is on the home page

Steps:
1. Observe quick access buttons

Expected Result:
- Buttons are visible: Task Board, Create Task, Search Tasks, RESTful API


### TC-006 - Task board structure
Preconditions:
- User is on the home page

Steps:
1. Click "Task Board"
2. Observe boards

Expected Result:
- Boards are displayed in order: Open → In Progress → Done


### TC-007 - Task content validation
Preconditions:
- User is on Task Board page

Steps:
1. Observe tasks

Expected Result:
- Each task contains:
  - Title
  - Description
  - Action buttons (View, Edit)


### TC-008 - Access Task Board via side menu
Preconditions:
- User is on the home page

Steps:
1. Click "Task Board" from side menu

Expected Result:
- User is redirected to Task Board page


### TC-009 - Access Task Board via quick button
Preconditions:
- User is on the home page

Steps:
1. Click "Task Board" quick access button

Expected Result:
- User is redirected to Task Board page


### TC-010 - Create task with valid data
Preconditions:
- User is on the home page

Steps:
1. Click "Create Task"
2. Enter valid title
3. Enter valid description
4. Select board
5. Submit

Expected Result:
- Task is created successfully
- Task appears in selected board


### TC-011 - Create task without title
Preconditions:
- User is on Create Task page

Steps:
1. Leave title empty
2. Enter valid description
3. Select board
4. Submit

Expected Result:
- Error message is displayed: "Please enter a title"
- Task is not created


### TC-012 - Create task without description
Preconditions:
- User is on Create Task page

Steps:
1. Enter valid title
2. Leave description empty
3. Select board
4. Submit

Expected Result:
- Task is created successfully (if description is optional)


### TC-013 - Create task without selecting board
Preconditions:
- User is on Create Task page

Steps:
1. Enter valid title
2. Enter valid description
3. Do not select board
4. Submit

Expected Result:
- Error message is displayed: "Please select a board"
- Task is not created


### TC-014 - View task details
Preconditions:
- User is on Task Board page

Steps:
1. Click "View" on a task

Expected Result:
- Task details page is opened
- All task information is displayed


### TC-015 - Edit task title
Preconditions:
- User is on Task Board page

Steps:
1. Click "Edit"
2. Change title
3. Save changes

Expected Result:
- Task title is updated successfully


### TC-016 - Edit task description
Preconditions:
- User is on Task Board page

Steps:
1. Click "Edit"
2. Change description
3. Save changes

Expected Result:
- Task description is updated successfully


### TC-017 - Change task board
Preconditions:
- User is on Task Board page

Steps:
1. Click "Edit"
2. Change board
3. Save changes

Expected Result:
- Task is moved to selected board


### TC-018 - Search task by keyword
Preconditions:
- User is on Home page

Steps:
1. Click "Search Tasks"
2. Enter keyword
3. Click "Search"

Expected Result:
- Matching tasks are displayed


### TC-019 - Search results content validation
Preconditions:
- User performs a search

Steps:
1. Observe search results

Expected Result:
- Each result contains:
  - Task title
  - Board name
  - Description (if available)


### TC-020 - REST API access
Preconditions:
- User is on Home page

Steps:
1. Click "RESTful API" button

Expected Result:
- API documentation or endpoint page is displayed
- User can access CRUD endpoints for tasks


