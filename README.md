### Description of the school management project (Python)

---
This program is a school management system written in Python. The  main parts of the school, like student, teacher, course, and classroom each have their own  class. Data is stored in a `data.json` file. When the program starts, information is loaded from this file, and after every change, the updated data is saved back into it.

#### Class structure

- The Course class includes the course ID,  name,  units, and scores.
- The Student class includes an ID, first name, last name, and a list of selected courses  with  grades.
- The Teacher class includes a teacher ID, first name, last name, grade, and the  courses they can teach.
- The Classroom class includes a classroom ID,  name,  assigned course, teacher, and  enrolled students.

#### Instruction
This program has multiple menus. You can perform different actions or open each menu by entering the number corresponding to the desired option. These menus are categorized and designed to be practical and simple, so everyone can use the application easily.

This program uses a step-by-step menu system controlled by the `level` variable. The user types a number to navigate to the corresponding menu, such as students, teachers, courses, or classrooms. At any time, the user can enter the number 0 to return to the previous menu.

When you run the program, the following main menu is displayed:
```
1.students
2.teachers
3.courses
4.classrooms
5.save
0.exit
```

For example, if you select Students, the following menu will open, allowing you to add, edit, delete, view, or select students:
```
1.add student
2.edit student
3.delete student
4.view students
5.select student
0.back
```

To use other menus, simply enter 0 to return to the main menu, then enter the number of the desired menu.
To exit the program, return to the main menu and enter 0, as shown in the example below:
```
1.add classroom
2.edit classroom
3.delete classroom
4.view classrooms
5.select classroom
0.back
>>0
1.students
2.teachers
3.courses
4.classrooms
5.save
0.exit
>>0
```