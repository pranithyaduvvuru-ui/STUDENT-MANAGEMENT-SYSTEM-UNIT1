# STUDENT-MANAGEMENT-SYSTEM-UNIT1
This repository contains the implementation of a Student Management System developed as part of Unit 1 coursework. The project focuses on the fundamental concepts of programming and object-oriented design by building a simple system to manage student data efficiently.  
# 🎓 Student Management Program (Java)

## 📌 Description

This is a simple Java program that demonstrates **Object-Oriented Programming (OOP)** concepts using a `Student` class.
The program allows the user to:

* Enter details of multiple students
* Store them using an array of objects
* Display all student details

---

## 🚀 Features

* Uses **classes and objects**
* Accepts **user input** using `Scanner`
* Stores multiple student records
* Displays formatted output

---

## 🛠️ Technologies Used

* Java
* OOP Concepts (Class, Object, Constructor)
* Arrays
* Scanner (for input)

---

## 📂 Code

```java
import java.util.*;

class Student {
    String name;
    int age;
    String department;
    long mobile;
    String address;
    String mail;

    Student(String a, int b, String c, long d, String e, String f) {
        this.name = a;
        this.age = b;
        this.department = c;
        this.mobile = d;
        this.address = e;
        this.mail = f;
    }

    void displayStudentdetail() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Department: " + department);
        System.out.println("Mobile No: " + mobile);
        System.out.println("Address: " + address);
        System.out.println("E-Mail: " + mail);
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);

        System.out.println("Enter number of students:");
        int n = s.nextInt();
        s.nextLine();

        Student[] detail = new Student[n];

        for (int i = 0; i < n; i++) {
            System.out.println("Enter details of student " + (i + 1));

            String name = s.nextLine();
            int age = s.nextInt();
            s.nextLine();
            String department = s.nextLine();
            long mobile = s.nextLong();
            s.nextLine();
            String address = s.nextLine();
            String mail = s.nextLine();

            detail[i] = new Student(name, age, department, mobile, address, mail);
        }

        for (int i = 0; i < n; i++) {
            System.out.println();
            detail[i].displayStudentdetail();
        }
    }
}
```

<img width="1600" height="611" alt="1" src="https://github.com/user-attachments/assets/daf3ccb7-0089-47a1-abb0-243edfdafa0d" />
<img width="1600" height="601" alt="2" src="https://github.com/user-attachments/assets/23bc78d7-fd1c-41e1-ba28-f69c94e392ab" />
<img width="1600" height="610" alt="3" src="https://github.com/user-attachments/assets/593cb34c-91a4-4719-84be-d91b2256c42c" />

---

## ▶️ How to Run

1. Save the file as `Main.java`
2. Open terminal or command prompt
3. Compile the program:

   ```bash
   javac Main.java
   ```
4. Run the program:

   ```bash
   java Main
   ```

---

## 📥 Sample Input

```
Enter number of students:
1
Enter details of student 1
Pranithya
20
CSE
9876543210
Chennai
pranithya@gmail.com
```

---

## 📤 Sample Output

```
Name: Pranithya
Age: 20
Department: CSE
Mobile No: 9876543210
Address: Chennai
E-Mail: pranithya@gmail.com
```

---

## 📚 Concepts Covered

* Class and Object creation
* Constructor usage
* Array of objects
* User input handling

---

## ✨ Future Improvements

* Add validation for input
* Store data in files or database
* Add menu-driven options (Add, Delete, Search)
* Use GUI (Swing/JavaFX)

---

## 📄 License

This project is free to use for educational purposes.

---
