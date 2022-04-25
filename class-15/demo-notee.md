# dn-class-16-demo

## today Topics

  1. DTOs

  2. Swagger

  3. testing

  4. maybe deployment

------------------------

- api/students

- respones comes from DB and class

- the keys comes from the DB

------------------------

- EX: login system (id, username, Email)those kesy are sensitive data Hacker should not see they may delete some records

------------------------

- techID is not usefull should be the name of the tech

------------------------

## what are DTOs?

- is a way to shape our data (API Schema)

- why we need it?

- sometimes we need in the front end a 5 props but the backecd object have more than 15 props

------------------------

## prep Coding

- in students controller

- in api/students(/2) note that we are returning a list of students/student and will change it to shaped students/student object

------------------------

- where we get the students/student from?

- what are the Get students/student dose?

- what dose the LinQ query do?

------------------------

- in GetStudents(GetStudent): it will return a shaped list of Students/Student (DTOs)

------------------------

## Coding

### StudentDto & CourseDto

- DTO Folder in models ==> StudentDto file  ==> add props ==> CourseDto ==> add props

- run to get Befor and After (screenshoot)

------------------------

- in Student controller change the Type from Student to StudentDto for both Gets

- ask what to change? ==> StudentDto in interface

------------------------

- in GetStudent service

- change the LinQ ==> first just the Student ==> run ==> then the Courses ==> run

- ask how to get Tech name ==> add the Nav Prop ==> run

------------------------

- in GetStudent do the same

------------------------

### NewStudentDto also add him to course

- NewStudentDto file  ==> add props

- in Student controller change the type to studentDto==> and the args to NewStudentDto ==> also interface

- in create service ==> add new studen obj

- now I have studentID but I do not have the courseID??

- in cource service add the GetCourseByCode service ==> add it to interface

- add the _course ==> ask it look like waht

- add the Course dependency

- complete what after the new studen obj ==> use getStudent to fix the return

- fix the student controller ==> run postman
