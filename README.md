# Library-Manageent-System
Library Management System is a menu-driven Java application designed to automate the basic operations of a library. The system maintains a catalog of books and registered members, allowing a librarian to add or remove books, search for books, register members, issue books, return books, and monitor overdue loans.
What it does
Manages a book catalog and a list of members, and lets a librarian issue and return books. Each loan gets a 14-day due date, and
returning a book late calculates a fine (5 per day late). Everything is saved to plain text files on exit and loaded back in on the next
run.
Menu options
• Add a book (or add more copies of one that already exists)
• Remove a book (blocked if copies are still on loan)
• List all books / search by title
• Register a member
• List members
• Issue a book to a member
• Return a book (shows fine if late)
• View a member's active loans
• View all overdue books
Classes
Book.java
Book data: ISBN, title, author, copy counts
Member.java
Member data: ID, name, email
Transaction.java
One issue/return record with dates
LibraryException.java
Custom exception for error cases (book not found, no copies left, etc.)
FileManager.java
Reads/writes the text files
Library.java
All the actual logic - issuing, returning, fines, checks
LibraryManagementSystem.java
Main class - the menu and user inpu
