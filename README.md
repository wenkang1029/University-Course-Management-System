# University Course Management System

A comprehensive Object-Oriented Programming (OOP) project that demonstrates advanced Java concepts through a university course management system. This system manages students, courses, instructors, and various administrative operations using core OOP principles.

## 🎯 Project Overview

This project is designed as part of an Object-Oriented Programming course to showcase the implementation of key OOP concepts including:
- **Inheritance** - Base Person class extended by Student and Instructor
- **Polymorphism** - Method overriding and interface implementations
- **Encapsulation** - Private fields with public getter/setter methods
- **Abstraction** - Abstract classes and interfaces for common behaviors
- **Composition** - Complex relationships between classes

## 🏗️ System Architecture

### Core Classes

#### Base Classes
- **`Person`** - Abstract base class for all individuals in the system
- **`Course`** - Represents academic courses with enrollment management
- **`Department`** - Manages courses and faculty within academic departments

#### Derived Classes
- **`Student`** - Extends Person, manages enrollments and academic records
- **`Instructor`** - Extends Person, handles course assignments and teaching
- **`Administrator`** - Extends Person, manages system-wide operations

#### Management Classes
- **`University`** - Central management system coordinating all operations
- **`EnrollmentManager`** - Handles student course enrollments
- **`GradeManager`** - Manages student grades and academic performance

## 🚀 Features

### Student Management
- ✅ Student registration and profile management
- ✅ Course enrollment and withdrawal
- ✅ Grade tracking and GPA calculation
- ✅ Academic transcript generation

### Course Management
- ✅ Course creation and scheduling
- ✅ Enrollment capacity management
- ✅ Prerequisite checking
- ✅ Course catalog browsing

### Instructor Management
- ✅ Instructor assignment to courses
- ✅ Grade submission and management
- ✅ Class roster access
- ✅ Student performance tracking

### Administrative Features
- ✅ Department management
- ✅ Academic calendar management
- ✅ Reporting and analytics
- ✅ System user management

## 📋 Prerequisites

- **Java Development Kit (JDK) 8 or higher**
- **IDE** (IntelliJ IDEA, Eclipse, or VS Code recommended)
- **Git** for version control

## 🛠️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/University-Course-Management-System.git
   cd University-Course-Management-System
   ```

2. **Compile the project**
   ```bash
   javac -d bin src/*.java
   ```

3. **Run the application**
   ```bash
   java -cp bin Main
   ```

## 💻 Usage

### Running the System

The system provides an interactive console interface for testing various functionalities:

```java
// Example: Creating and managing students
Student student = new Student("John Doe", "S001", "Computer Science");
student.enrollInCourse(course);
student.displayTranscript();

// Example: Managing courses
Course course = new Course("CS101", "Introduction to Programming", 3);
course.addStudent(student);
course.displayEnrolledStudents();
```

### Key Operations

1. **Student Operations**
   - Register new students
   - Enroll in courses
   - View grades and transcripts
   - Calculate GPA

2. **Course Operations**
   - Create new courses
   - Manage enrollments
   - Set prerequisites
   - Generate class lists

3. **Instructor Operations**
   - Assign to courses
   - Submit grades
   - View student performance
   - Generate reports

## 🎓 OOP Concepts Demonstrated

### 1. Inheritance
```java
public abstract class Person {
    // Base implementation
}

public class Student extends Person {
    // Student-specific implementation
}
```

### 2. Polymorphism
```java
Person person = new Student(); // Runtime polymorphism
person.displayInfo(); // Calls Student's overridden method
```

### 3. Encapsulation
```java
private String studentId;
public String getStudentId() { return studentId; }
public void setStudentId(String id) { this.studentId = id; }
```

### 4. Abstraction
```java
public interface Enrollable {
    void enroll(Student student);
    void withdraw(Student student);
}
```

## 📁 Project Structure

```
University-Course-Management-System/
├── src/
│   ├── Person.java              # Abstract base class
│   ├── Student.java             # Student implementation
│   ├── Instructor.java          # Instructor implementation
│   ├── Administrator.java       # Administrator implementation
│   ├── Course.java              # Course management
│   ├── Department.java          # Department management
│   ├── University.java          # Main system controller
│   ├── EnrollmentManager.java   # Enrollment operations
│   ├── GradeManager.java        # Grade management
│   └── Main.java                # Application entry point
├── bin/                         # Compiled classes
├── docs/                        # Documentation
└── README.md                    # Project documentation
```

## 🧪 Testing

The project includes comprehensive testing scenarios in the `Main.java` file:

- Student registration and management
- Course creation and enrollment
- Grade assignment and calculation
- Department and university operations
- Error handling and validation

## 🤝 Contributing

This is an educational project for OOP course demonstration. If you'd like to contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request

## 📚 Learning Objectives

This project demonstrates:
- **Class Design** - Proper class hierarchy and relationships
- **Data Encapsulation** - Protecting data integrity
- **Method Overriding** - Customizing behavior in derived classes
- **Interface Implementation** - Achieving abstraction
- **Exception Handling** - Robust error management
- **Collection Framework** - Managing groups of objects

## 📄 License

This project is created for educational purposes as part of an Object-Oriented Programming course.

## 👨‍💻 Author

**Your Name**
- GitHub: [@wenkang1029](https://github.com/wenkang1029)
- Course: Object-Oriented Programming

## 🙏 Acknowledgments

- Course instructor and teaching assistants
- Java documentation and tutorials
- Object-Oriented Programming concepts and best practices

---

*This project serves as a practical implementation of OOP principles and demonstrates real-world application of software engineering concepts in an educational context.*