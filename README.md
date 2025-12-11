### Description of the school management project (Python)

---
This program is a school management system written in Python. The  main parts of the school - student, teacher, course, and classroom - each have their own  class. Data is stored in a `data.json` file. When the program starts, information is loaded from this file, and after every change, the updated data is saved back into it.

#### Class Structure

- The Course class includes the course ID,  name,  credits, and student grades.
- The Student class includes an ID, first name, last name, and a list of selected courses  with  grades.
- The Teacher class includes a teacher ID, first name, last name, grade, and the  courses they can teach.
- The Classroom class includes a classroom ID,  name,  assigned course, teacher, and  enrolled students.

#### Data Loading and Management

At the start of the program, data is read from the JSON file. Each section  is converted into Python objects and stored in separate lists.
When adding, editing, or deleting  data, the program  checks for invalid or conflicting information. 

- A course can't be deleted if it's still assigned to a student or  teacher.
- A student can only be added to a classroom if they have the course and their grade is below 10.
- A teacher can only be assigned to a classroom if they're qualified to teach the course.

#### Menus and User Interaction

1. The system uses multi-level menus.
2. Users can add, edit, or delete students.
3. They can assign courses  and enter  grades.
4. Users can register new teachers or edit their courses.
5. They can create new courses or manage existing ones.
6. Users can create classrooms, change the assigned teacher or course, and add or remove students.
7. Finally, use the Save option to write all updated data back to the JSON file.