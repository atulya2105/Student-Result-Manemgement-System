# Student-Result-Manemgement-System
 
Language used: SQL,Java.

Technology used: Java Swing, Java AWT, JDBC, DBUtils.

Software used: Apache Netbeans, MySQL.

## 1. HomePage
In this jframe there is two botton

-Admin - redirect to Admin login page(frame).

-Student - redirect to student portal(frame).

![image](https://user-images.githubusercontent.com/84077760/207152506-0e17dca5-f8eb-4a69-8eea-b6e342ce5e9b.png)

## 2. AdminIndex 
- In this jframe staff need to provide UserID and Password inorder to login into staff Home Page.
- As per this project I have kept the userID "admin" and password "admin" to login.
![image](https://user-images.githubusercontent.com/84077760/207153471-645eb935-9438-41a1-9a29-99a280ad0398.png)

## 3. AdminHome
As soon as the staff click on login it redirect to Staff Home Page where staff can perform following operation.
a) Add New Student
b) Insert New Result
c) Registered Student
d) All Student Result

The above all bottons will be present in StaffHomepage, InsertNewResult, RegisteredStudent and AllStudentResult jFrames.

Add New Student

- By default the staff home page has this frame where staff can enter student basic detail like roll number(this should be unique), name, class, date of birth, gender,father name.
- As soon as we click on add all the details will be stored in mysql database of table name "student" inside school databaser with respect to "rollNumber" as a primary key.
- Before adding the data in student table please create a table "student" inside "school" database

create table student(rollnumber varchar(255) primary key, name varchar(255), studentclass int, dob varchar(255), gender char(4), fathername varchar(255));
![image](https://user-images.githubusercontent.com/84077760/207155623-c20c0b71-1187-433c-8944-6041c700cfb1.png)

- Note: In these project I have used user name as "root" and password as "root". Please enter your MySQL password inside all the jframe where ever database is used.

![image](https://user-images.githubusercontent.com/84077760/207153137-ff8c94e3-50eb-4c85-9c07-a46f46c8cce6.png).

## 4. Insert New Result
- Inorder to add the marks of student. Staff need to click on "Insert New Result" botton.
- First need to enter the student roll number and click on search button so that student name will be displayed to verify.
- Now Admin can enter the student marks
- Before adding the data in student table please create a table "result" inside "school" database.

create table result(rollnumber varchar(255) primary key, kannada int, english int, hindi int, mathematics int,science int, social int);
![image](https://user-images.githubusercontent.com/84077760/207156061-a9d56827-77aa-4c5a-a1ea-d30db32c30bf.png)

- Once the staff click on add. The marks of the students in all the subject will be saved in school database in table name "result" with respect to "rollnumber" as a primary key.
![image](https://user-images.githubusercontent.com/84077760/207156393-159233fc-09e7-474b-b6f1-9b32ca899686.png)

## 5. Rgistered Student

- As the staff click on Registered Student. All the details of Students will be fetched from database and displayed. As shown below.
![image](https://user-images.githubusercontent.com/84077760/207156754-de5a8ae0-ab04-4d11-b3c7-cfd996539a0b.png)

## 6. All Student Result 
 - Similarly as the staff click on All Student Result. All the subject marks of Students will be fetched from database and displayed. As shown below.
 
 ![image](https://user-images.githubusercontent.com/84077760/207156956-77cb5a08-1086-4336-8dcf-60268f773cc9.png)
 
 ## 7. Student Portal
 
- Student will be redirected to Student portal when clicked on Student botton in Home page.
- Student need to enter the valid rollnumber to fetch the result else "Invalid Roll Number" message will popup.
- If Students enters the valid roll number then it will be redirected to StudentResult page.

![image](https://user-images.githubusercontent.com/84077760/207157283-77e7c2b8-d531-448d-b699-0a214493cc2c.png)

## 8. Result 

- This is the frame where the result of student will be displayed.

- Below is the two example where one student is passed and other student is failed.
![image](https://user-images.githubusercontent.com/84077760/207157489-73563193-a327-4e8c-ac7c-5499e07f9745.png)


# Thank You!
 
 










