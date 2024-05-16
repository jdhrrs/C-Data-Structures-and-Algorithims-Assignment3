# Assignment3

## Overview
This project implements a Stack data structure using a linked list in C++. It manages `Person` objects, which include `Address` details. The project consists of several C++ files organized into logical units for handling persons, addresses, and stack operations.

## File Structure
`Address.h` / `Address.cpp`
- These files define and implement the `Address` class, which includes information such as street, city, state, and zip code.

`Person.h` / `Person.cpp`
- These files define and implement the `Person` class, which includes personal information such as name and an `Address` object.

`Node.h`
- This file defines the `Node` class used in the stack, representing each element in the list.

`Stack.h` / `Stack.cpp`
- These files define and implement the `Stack` class, which manages a collection of `Node` objects. Each `Node` contains a `Person` object and a pointer to the next node.

`main.cpp`
- This file contains the main function, which serves as the entry point of the program. It demonstrates the usage of the `Stack` to manage the stack operations.

## Classes
### Address
**Attributes:**
- street: std::string
- city: std::string
- state: std::string
- zip: std::string

**Methods:**
- Constructors
- Getters and setters for each attribute
- print(): Displays the address information

### Person
**Attributes:**
- name: std::string
- address: Address

**Methods:**
- Constructors
- Getters and setters for each attribute
- print(): Displays the person's information, including their address

### Node
**Attributes:**
- person: Person
- next: Node* (pointer to the next node)

**Methods:**
- Constructors

### Stack
**Attributes:**
- top: Node* (pointer to the top node in the stack)

**Methods:**
- push(Person p): Adds a person to the stack
- pop(): Removes the top person from the stack
- isFull(): Checks if the stack is at its capacity
- print(): Displays all persons in the stack

## Getting Started

### Prerequisites
- C++ compiler (e.g., g++)

### Compilation and Execution
Compile the project using the following command:
g++ -o stack main.cpp Address.cpp Person.cpp Stack.cpp


## Usage
The program demonstrates adding and removing persons from the stack, checking if the stack is full, and printing the list of all persons.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- Instructor: Prof. Professor.Randall Hutton
- Course: COSC 350 - Advanced Algorithms and Data Structures, Columbia College of Missouri

