# API Data Handling and Exporting

In this project, we focus on fetching data from a REST API, processing the data, and exporting it in various formats.

## Tasks

### 0. Gather data from an API

**Objective:**
Write a Python script that, using the REST API, returns information about an employee's TODO list progress based on their employee ID.

**Requirements:**
- Use either the `urllib` or `requests` module.
- The script should accept an integer (employee ID) as an argument.
- The script should display the employee's TODO list progress on the standard output in the specified format.

**Usage Example:**
```bash
$ python3 0-gather_data_from_an_API.py 2
```

**GitHub Repository:** `holbertonschool-back-end`
**Directory:** `api`
**File:** `0-gather_data_from_an_API.py`

### 1. Export to CSV

**Objective:**
Extend the script from task #0 to export the data in CSV format.

**Requirements:**
- Record all tasks owned by the employee.
- Format: "USER_ID","USERNAME","TASK_COMPLETED_STATUS","TASK_TITLE"
- File name: `USER_ID.csv`

**Usage Example:**
```bash
$ python3 1-export_to_CSV.py 2
```

**GitHub Repository:** `holbertonschool-back-end`
**Directory:** `api`
**File:** `1-export_to_CSV.py`

### 2. Export to JSON

**Objective:**
Extend the script from task #0 to export the data in JSON format.

**Requirements:**
- Record all tasks owned by the employee.
- Format: `{ "USER_ID": [{"task": "TASK_TITLE", "completed": TASK_COMPLETED_STATUS, "username": "USERNAME"}, ...] }`
- File name: `USER_ID.json`

**Usage Example:**
```bash
$ python3 2-export_to_JSON.py 2
```

**GitHub Repository:** `holbertonschool-back-end`
**Directory:** `api`
**File:** `2-export_to_JSON.py`

### 3. Dictionary of list of dictionaries

**Objective:**
Extend the script from task #0 to export data for all employees in the JSON format.

**Requirements:**
- Record tasks from all employees.
- Format: `{ "USER_ID": [ {"username": "USERNAME", "task": "TASK_TITLE", "completed": TASK_COMPLETED_STATUS}, ... ], ... }`
- File name: `todo_all_employees.json`

**GitHub Repository:** `holbertonschool-back-end`
**Directory:** `api`
**File:** `3-dictionary_of_list_of_dictionaries.py`
