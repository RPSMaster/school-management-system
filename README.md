### Description of the school management project (Python)

---
This program is a school management system written in Python. The  main parts of the school, like student, teacher, course, and classroom each have their own  class. Data is stored in a `data.json` file. When the program starts, information is loaded from this file, and after every change, the updated data is saved back into it.

#### Class structure

- The Course class includes the course ID,  name,  units, and scores.
- The Student class includes an ID, first name, last name, and a list of selected courses  with  grades.
- The Teacher class includes a teacher ID, first name, last name, grade, and the  courses they can teach.
- The Classroom class includes a classroom ID,  name,  assigned course, teacher, and  enrolled students.

#### Instruction
This program uses a step-by-step menu system controlled by the `level` variable. The user types a number to go to the matching menu, like students, teachers, courses, or classrooms. The user can enter the number 0 to return to the previous menu. For example:
``` python
1.students
2.teachers
3.courses
4.classrooms
5.save
0.exit
>>1
1.add student
2.edit student
3.delete student
4.view students
5.select student
0.back
>>0
1.students
2.teachers
3.courses
4.classrooms
5.save
0.exit
>>4
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