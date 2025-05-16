Password Manager

🌟 Welcome to the Password Manager! 🌟This is a simple, console-based Python application designed to manage user details like names, usernames, and passwords. Perfect for Python beginners or anyone looking to organize credentials in a straightforward way, this script offers a menu-driven interface to add, display, and verify user data. Let’s explore how this tool can help you learn Python and manage information with ease!
This README covers everything you need to know about the project, from setup to contributing. Ready to dive in? Let’s go! 🚀

Table of Contents

Features
How It Works
Installation
Usage
Sample Output
Known Issues
Contributing
License
Call to Action


Features

Add User Details: Input name, username, and password for storage.
Display Details: View the most recently entered user information.
Credential Verification: Check if a username and password match the stored data.
Simple Menu Interface: Choose from four options (Add, Show, Verify, Exit) via a console menu.
Input Validation: Handles invalid inputs with clear error messages.
Scalable Loop: Supports multiple operations in a session (up to 99,999 iterations).


How It Works
The Password Manager is a Python script that uses a list (data) to track user interactions and provides a menu-driven interface. Here’s the breakdown:

Welcome Banner: Displays a centered “Welcome to The Password Manager” message using string.center().
Menu Options:
1. Add Details: Prompts for name, username, and password, then appends the choice to the data list (currently only stores the choice, not the details).
2. Show Detail: Displays the last entered name, username, and password (references variables that may be undefined if no data exists).
3. User and Password Match: Verifies if the entered username and password match the last stored credentials.
4. Exit: Exits the program with a goodbye message.


Error Handling: Rejects invalid inputs (outside 1-4) with a prompt to try again.
Loop Structure: Runs in a loop (1 to 99,999) to allow multiple operations per session.

Note: The script has some limitations, like not storing user details correctly and referencing undefined variables. See Known Issues and Contributing for details on improving it.

Installation
Setting up the Password Manager is quick and easy! Follow these steps:

Prerequisites:

Python 3.x installed (Download Python).
A code editor like VS Code, PyCharm, or Notepad (optional).


Clone the Repository:
git clone https://github.com/codewithjatin70/Password-Manager
cd password-manager


Save the Script:

Copy the provided Python code into a file named password_manager.py.
Alternatively, download password_manager.py from this repository (once uploaded).


Run the Script:
python password_manager.py



No external libraries needed—just pure Python! 🐍

Usage
After running the script, you’ll see a welcome banner and a menu with four options. Here’s how to use each:

Add Details (Option 1):

Enter your name, username, and password.
The script confirms with “Details added successfully!” (Note: Details aren’t stored in data yet—see Known Issues).


Show Detail (Option 2):

Displays the last entered name, username, and password (if defined).


User and Password Match (Option 3):

Enter a username and password to check if they match the last stored credentials.
Outputs “Your password is match” or “Your password not match”.


Exit (Option 4):

Exits the program with “Exiting program. Goodbye!”.



Example Workflow

Run python password_manager.py.
See the menu: 1. Add Details, 2. Show Detail, 3. User and Password Match, 4. Exit.
Choose 1, enter details (e.g., Name: Priya, Username: priya123, Password: pass123).
Choose 3, verify (e.g., Username: priya123, Password: pass123 → “Your password is match”).
Choose 4 to exit.


Sample Output
************************Welcome to The Password Manager************************

  1. Add Details
  2. Show Detail
  3. User and Password Match
  4. Exit
Enter you chioce : 1
Enter your name : Priya Sharma
Enter your username : priya123
Enter your password : pass123
Details added successfully!

  1. Add Details
  2. Show Detail
  3. User and Password Match
  4. Exit
Enter you chioce : 2
--- Entry 1 ---
Name : Priya Sharma
Username : priya123
Password : pass123

  1. Add Details
  2. Show Detail
  3. User and Password Match
  4. Exit
Enter you chioce : 3
Enter your user name : priya123
Enter your user password : pass123
Your password is match

  1. Add Details
  2. Show Detail
  3. User and Password Match
  4. Exit
Enter you chioce : 4
Exiting program. Goodbye!


Known Issues
The script is functional but has a few areas for improvement:

Data Storage: The data list only stores the chioce (e.g., “1”), not the name, username, or password. This limits the ability to retrieve or display multiple entries.
Undefined Variables: Options 2 and 3 reference name, username, and password, which may be undefined if option 1 hasn’t been used first, causing errors.
Single Entry: The script only tracks the latest entry, not a history of all users.
Security: Passwords are stored in plain text, which isn’t secure for real-world use.
Typo in Code: “chioce” should be “choice” for clarity.

See Contributing for how to fix these!

Contributing
We’d love your help to make this Password Manager even better! Here are some ideas to improve it:

Fix Data Storage: Store name, username, and password in the data list as a dictionary (e.g., data.append({"name": name, "username": username, "password": password})).
Display All Entries: Update option 2 to show all stored entries, not just the latest.
Add File Storage: Save data to a file (e.g., JSON or CSV) for persistence across sessions.
Secure Passwords: Use hashlib to hash passwords for better security.
Robust Error Handling: Prevent crashes by checking if variables are defined before use.
Fix Typos: Correct “chioce” to “choice” and improve grammar in prompts (e.g., “Your password is match” → “Your password matches”).

To contribute:

Fork the repository.
Create a branch (git checkout -b fix-data-storage).
Commit changes (git commit -m "Fixed data storage with dictionaries").
Push to your fork (git push origin fix-data-storage).
Open a Pull Request.

Let’s make this tool awesome together! 🙌

License
This project is licensed under the MIT License. Feel free to use, modify, and share it!
