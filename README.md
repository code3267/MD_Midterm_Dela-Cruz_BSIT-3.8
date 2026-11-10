educational purposes


NAME:kurt ahron dela cruz BSIT3.8
# Community Learning Center Management System

## Application Overview
The Community Learning Center Management System is a Dart console application that manages learning resources (books and equipment) and center participants. The system provides an interactive 4-option menu to register records, manage inventory, and display structured data while implementing core object-oriented programming principles in Dart.

## Implemented Features
* Program Setup & I/O: Interactive console menu with input validation and conditional logic.
* Control Structures & Error Handling: Loops, switch statements, and try-catch blocks to prevent unexpected application termination.
* Encapsulation & Collections: Private fields with getters/setters, paired with List and Map collections to store and retrieve records.
* Inheritance & Polymorphism: An abstract parent class (`CenterRecord`) extended by specialized subclasses (`BookResource`, `EquipmentResource`) demonstrating method overriding and polymorphic execution.
* Mixins: A custom `Timestampable` mixin that automatically attaches creation timestamps to records.

## Menu Options
1. Add Resource: Register a new Book or Equipment item.
2. Register Participant: Add a new center participant with a unique ID.
3. View Records: Display all registered resources (polymorphically) and participants.
4. Exit: Terminate the application loop safely.

## Sample Test Scenarios
1. Add Resource & Participant: Select Option 1 to add a Book (`B002`, `Clean Code`, `Robert Martin`, `3`). Select Option 2 to register a Participant (`P002`, `Jane Doe`, `Student`). Select Option 3 to verify both display properly.
2. Duplicate Key Validation: Select Option 2 and attempt to register a participant using an existing ID (`P001`). The system displays an error message and prevents duplicate insertion.
3. Invalid Menu / Numeric Input: Enter non-numeric input or an out-of-range number (e.g., `9` or `abc`) at the menu prompt. The system catches the error gracefully and prompts the user again without crashing.

## Instructions for Running the Program
1. Ensure the Dart SDK is installed on your environment.
2. Open the terminal in the root directory containing `main.dart`.
3. Run the application using:
   ```bash
   dart run main.dart

