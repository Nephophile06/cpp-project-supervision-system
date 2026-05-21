# 🎓 Project Supervision System (PSS)

A console-based **Project Supervision System (PSS)** built with **C++**. This project was developed as an academic management tool to help students register, manage their profiles, and submit project details, while allowing administrators to supervise registered students and view submitted projects.

This project strongly demonstrates core **Object-Oriented Programming (OOP)** concepts such as Inheritance, Encapsulation, and Data Hiding.


## 🚀 Features & Functionalities

The system is divided into two main modules: **User (Student)** and **Admin**.

### 👤 User (Student) Features

* **User Registration:** New students can create an account by providing their Name, ID, Department, Section, Batch, and a secure password.
* **Secure Login & Logout:** Registered users can log in using their credentials (Name, ID, and Password). The system prevents multiple logins at the same time.
* **Profile Management:** * **View Profile:** Users can view their registered details.
* **Edit Profile:** Users can update their Department, Section, and Password.


* **Task/Project Submission:** Logged-in users can add new projects by providing a "Project Name" and a "Short Description".

### 🛡️ Admin Features

* **Admin Login & Logout:** Dedicated secure login for administrators. *(Note: Admin credentials are hardcoded into the system).*
* **View Registered Students:** Admins can view a complete, detailed list of all the students registered in the system.
* **View Project List:** Admins can monitor all the projects/tasks submitted by the students.


## 💻 Technical Details & OOP Concepts Used

* **Language:** C++
* **Inheritance:** A base class `Person` is created to hold common attributes (like Name), which is inherited by both `User` and `Admin` classes.
* **Encapsulation:** Sensitive data (like passwords and task lists) are kept `private` and accessed only via getter/setter methods.
* **Dynamic Memory (Vectors):** The system uses `std::vector` to dynamically store user profiles and project tasks without predefined limits.
* **Session Management:** Tracks the currently logged-in user or admin using index pointers to prevent overlapping sessions.


## 🛠️ How to Run the Project

### Prerequisites

You need a C++ compiler installed on your system (e.g., GCC/MinGW for Windows, Clang for macOS).

### Steps to Compile and Execute

1. Save the source code in a file named `main.cpp`.
2. Open your terminal or command prompt.
3. Compile the code using the following command:
```bash
g++ main.cpp -o pss_app

```


4. Run the executable:
* **On Windows:**
```bash
pss_app.exe

```


* **On Linux/macOS:**
```bash
./pss_app

```

## 🔑 Default Admin Credentials

To access the Admin Panel, use the following default credentials:

* **Admin Name:** `Shifa`
* **Admin Code/Password:** `123456`

## ⚠️ Limitations

* **In-Memory Storage:** This project currently uses vectors for storage. All data (registered users and projects) is temporarily stored in the RAM and will be lost once the application is closed.
* **Future Scope:** File handling (`fstream`) or a Database connection can be integrated to make the data permanent.
