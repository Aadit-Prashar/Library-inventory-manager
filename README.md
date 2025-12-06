**📚 Library Management System**
Project Overview
The Library Management System is a robust, CLI-based Python application designed to manage book inventories efficiently. It demonstrates core software engineering principles including Object-Oriented Programming (OOP), file persistence with JSON, modular architecture, and exception handling
This systm allows librarians to manage their catalog, issue/return books, and persist data across sessions, ensuring no data is lost when the program closes.

**✨ Features**
📖 Book Management: Add new books with details like Title, Author, and ISBN.
🔄 Circulation System: Issue books to members and accept returns, updating status in real-time.
💾 Data Persistence: Automatically saves and loads the inventory using a JSON database (library.json), ensuring data integrity.
🔍 Search Functionality:

Search for books by Title (case-insensitive partial match).
Find specific books by ISBN.

🛡️ Robust Error Handling: graceful handling of missing files, corrupted data, and invalid user inputs.

📝 Logging: Tracks important events and errors in a library.log file for debugging and auditing.

✅ Modular Design: Organized into separate modules for logic (library_manager) and interface (cli).

📂 Project Structure
LibraryProject/
├── library_manager/ # Core Logic Package
│ ├── **init**.py
│ ├── book.py # Book Class & Attributes
│ └── inventory.py # Inventory Management & JSON I/O
├── cli/ # User Interface Package
│ └── main.py # Main Entry Point
├── tests/ # Unit Tests
│ └── test.py
├── library.json # Database (Auto-generated)
├── library.log # Log File (Auto-generated)
├── requirements.txt # Dependencies
└── README.md # Project Documentation
🚀 Getting Started
Prerequisites

Python 3.x installed on your system.
Installation

Clone or download this repository.

Navigate to the project directory:

cd LibraryProject
(Optional) Install test dependencies:
pip install -r requirements.txt


**💻 Usage**
To start the application, run the main.py script from the project root:

python cli/main.py
Using the Menu:

Add Book: Enter the book details. Duplicate ISBNs are prevented.

Issue Book: Mark a book as "issued" using its ISBN.

Return Book: Mark a book as "available" using its ISBN.

Search: Find books by title keywords.

View All: Display the entire catalog.

Exit: Close the program (data is saved automatically).


AUTHOR:Aadit Prashar
Date:5/12/2025
