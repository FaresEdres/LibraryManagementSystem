# Library Management System

## Overview
This project demonstrates the integration of Object-Oriented Programming (OOP), exception handling, generics, and wildcards in Java. It implements a simple yet comprehensive Library Management System that includes:

- A class hierarchy for library items and clients.
- Custom exception handling for error scenarios.
- Create, Read and Delete operations.
- Borrowing and returning items functionality.
- Use of Java Streams for efficient data processing.
- A user-friendly menu-driven interface.

## Features

### 1. Library Items
- **Class Hierarchy**:
  - Abstract class `LibraryItem` with properties like `id` and `title`.
  - Subclasses `Book` and `Magazine` that extend `LibraryItem`.
  - Method `getItemDetails()` to retrieve item details.
- **Generics and Wildcards**:
  - Manage collections of any `LibraryItem` subclass.
  - Methods for adding, retrieving, and displaying items.

### 2. Library Clients
- **Class Design**:
  - `Client` class with properties like `id`, `name`, and `email`.
  - Method `getClientDetails()` to display client information.
- **Relation with Library Items**:
  - Each client can borrow multiple library items.

### 3. Exception Handling
- **Custom Exception**:
  - `ItemNotFoundException` is thrown when a requested library item is not found.
  - `clientNotFound` is thrown when a requested client is not found.

### 4. Borrow and Return Features
- **Methods**:
  - `borrowItem(userId, itemId)`: Allows a client to borrow an item.
  - `returnItem(itemId, userId)`: Allows a client to return an item.

### 5. Java Streams
- **Efficient Data Handling**:
  - Use streams to filter library items, find clients by ID, and perform other operations efficiently.

### 6. Validations
- Ensure unique IDs for all entities (`LibraryItem` and `Client`).
- Validate user inputs for correctness (e.g., item availability, valid IDs).


### 7. User-Friendly Menu
- Clear instructions for navigating the menu.
- Meaningful error messages for invalid operations.

## Setup and Usage

### Prerequisites
- Java Development Kit (JDK) 8 or later.
- Any IDE or text editor for Java development (e.g., IntelliJ IDEA, Eclipse).

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/LibraryManagementSystem.git
   ```
2. Open the project in your preferred IDE.
3. Compile and run the `Main` class.

### Running the Application
1. Start the application to access the menu system.
2. Use the menu options to:
   - Add or manage library items (Books, Magazines).
   - Add or manage library clients.
   - Borrow and return library items.
   - View item and client details.

## Assumptions
- Each `LibraryItem` and `Client` has a unique ID.
- Borrowing is only allowed if the item is available.
- The application supports basic error handling for invalid operations.

## Future Enhancements
- Add a database backend for persistent storage.
- Implement user authentication for accessing the system.
- Extend support for additional item types (e.g., DVDs, Journals).
- Enhance the UI with a graphical interface or a web application.

---


