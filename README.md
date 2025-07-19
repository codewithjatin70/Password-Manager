🔐 Password Manager – Python Console App

🌟 Welcome to the Password Manager! 🌟
A simple, console-based Python application designed to manage user credentials like name, username, and password. Perfect for Python beginners, this menu-driven app helps organize and verify login data in a clear and interactive way.


---

📄 Table of Contents

🚀 Features

⚙️ How It Works

📦 Installation

🧑‍💻 Usage

📊 Sample Output

🐞 Known Issues

🤝 Contributing

📄 License

📣 Call to Action



---

🚀 Features

➕ Add User Details: Store name, username, and password

👁️ Display Details: Show last entered credentials

✅ Credential Verification: Match username and password

🧭 Simple Menu: Choose from 4 options via terminal

🚫 Input Validation: Handles invalid entries gracefully

🔁 Scalable Loop: Supports repeated use within the session



---

⚙️ How It Works

The script uses variables and simple lists to hold user data. You interact with a menu to perform the following:

Menu Options:

1. Add Details – Enter your name, username, and password


2. Show Detail – Display the last entered credentials


3. Verify Credentials – Match entered username and password


4. Exit – Close the program gracefully



> The loop allows up to 99,999 operations per session.



> ℹ️ Note: The current script only stores the latest entry, not a list of users.




---

📦 Installation

Prerequisites:

Python 3.x

Any code editor (VS Code, PyCharm, etc.)


Steps:

git clone https://github.com/codewithjatin70/Password-Manager
cd Password-Manager

Create or download the script as password_manager.py, then run:

python password_manager.py

✅ No external libraries required — pure Python!


---

🧑‍💻 Usage

After launching, use the menu to:

➕ Add Details (Option 1)

Enter name, username, and password

Success message shown


👁️ Show Details (Option 2)

Displays the most recently stored credentials


🔐 Credential Match (Option 3)

Enter username and password

Returns match result


🚪 Exit (Option 4)

Gracefully exits with a goodbye message



---

📊 Sample Output

**************** Welcome to The Password Manager ****************

  1. Add Details
  2. Show Detail
  3. User and Password Match
  4. Exit

Enter your choice: 1
Enter your name: Priya Sharma
Enter your username: priya123
Enter your password: pass123
Details added successfully!

Enter your choice: 2
--- Entry 1 ---
Name     : Priya Sharma
Username : priya123
Password : pass123

Enter your choice: 3
Enter your username: priya123
Enter your password: pass123
✅ Your password matches!

Enter your choice: 4
Exiting program. Goodbye!


---

🐞 Known Issues

❌ Only the last user’s data is stored

❌ Variables undefined if Option 1 isn't used first

❌ Passwords are stored in plain text

📝 Typo: chioce → choice

📦 No persistence (data lost after exit)



---

🤝 Contributing

You're welcome to improve this project! Here are a few ideas:

🧠 Store user data using dictionaries in a list

🧾 Save to JSON or CSV for persistence

🔐 Use hashlib to encrypt passwords

👥 Support multiple users

✅ Fix typos, improve prompts


Steps:

git fork https://github.com/codewithjatin70/Password-Manager
git checkout -b feature-enhancement
# Make changes
git commit -m "Enhanced password verification and storage"
git push origin feature-enhancement

Open a Pull Request — let's build it together! 🚀


---

📄 License

This project is licensed under the MIT License.
Feel free to use, modify, and share it!


---

📣 Call to Action

💡 Star this repo
🐛 Report bugs or suggest improvements
🙌 Fork & contribute


---

Made with ❤️ by @codewithjatin70


---

