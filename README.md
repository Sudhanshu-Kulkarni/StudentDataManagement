# Student Management System

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Classes and Methods](#classes-and-methods)
- [How to Run](#how-to-run)

## Overview
This Student Management System allows users to perform basic operations such as adding, updating, deleting, and searching students by their PRN (Permanent Registration Number), Name, or Position. The program uses Java and handles various exceptions such as invalid menu choices and student not found errors.

The program includes the following main classes:
- **Main**: Contains the main logic for presenting a menu to the user and accepting input to perform actions based on the choice.
- **StudentOperations**: Contains methods to add, display, search, update, and delete student records. This class also handles custom exceptions.
- **Student**: Represents a student with a `name` and `prn` and includes methods to manage student information.

## Features
- **Add Student**: Allows the user to add a student by providing their Name and PRN.
- **Display All Students**: Displays details of all students in the system.
- **Search by PRN**: Search for a student by their unique PRN and display their details.
- **Search by Name**: Search for a student by their name (case-insensitive).
- **Search by Position**: Search for a student by their position in the list (1-based index).
- **Update Student**: Update the student's name using their PRN.
- **Delete Student**: Delete a student by their PRN.
- **Exit**: Exits the program.

## Classes and Methods

### Main Class
This class handles the main logic of the program by presenting a menu to the user and executing the corresponding operations.

- **Method: main(String[] args)**  
  The entry point of the program, where the user interacts with the menu and selects operations.

### StudentOperations Class
This class contains all the methods for managing students, such as adding, displaying, searching, updating, and deleting student records.

- **Method: addStudent(Student student)**  
  Adds a new student to the system.
  
- **Method: displayAllStudents()**  
  Displays all the students in the system.
  
- **Method: searchByPrn(String prn)**  
  Searches for a student by their PRN.
  
- **Method: searchByName(String name)**  
  Searches for students by their name (case-insensitive).
  
- **Method: searchByPosition(int position)**  
  Searches for a student based on their position in the list.
  
- **Method: updateStudent(String prn, String newName)**  
  Updates the student's name using their PRN.
  
- **Method: deleteStudent(String prn)**  
  Deletes a student from the system by their PRN.

### Student Class
Represents a student with basic attributes.

- **Constructor: Student(String name, String prn)**  
  Initializes a new student object with a name and PRN.

- **Method: String getName()**  
  Returns the student's name.

- **Method: String getPrn()**  
  Returns the student's PRN.

- **Method: void displayDetails()**  
  Displays the student's name and PRN.

## Custom Exceptions
The following exceptions are handled in the program:
1. **InvalidChoiceException**: Thrown when the user enters an invalid menu choice.
2. **DuplicateStudentException**: Thrown when trying to add a student with an existing PRN.
3. **StudentNotFoundException**: Thrown when a student is not found based on the search criteria.
4. **IndexOutOfBoundsException**: Thrown when an invalid position is entered while searching by position.
