# micro-mmorpg
A mmorpg
Odyssey of the Stars - Online Edition
=====================================

This folder contains the complete, portable game server and client files, ready for GitHub and cloud deployment.

---
### 1. System Requirements
---
- Python 3.8+
- MariaDB or MySQL Server

---
### 2. Setup Instructions
---
1.  **Install Python Dependencies:**
    Open your terminal or command prompt in this folder and run:
    `pip install Flask Flask-SocketIO mariadb werkzeug`

2.  **Set Up the Database:**
    - Make sure your MariaDB/MySQL server is running.
    - Run the database setup script from your terminal:
      `python databasecreator.py`
    - It will ask for your database 'root' user password to create the game database and tables.

3.  **Configure Database Connection:**
    - Open the `main_server.py` file in a text editor.
    - Find the `DB_CONFIG` dictionary near the top.
    - Change the 'password' value from 'your_root_password' to your actual MariaDB root password.

---
### 3. Running the Game
---
1.  **Start the Server:**
    Open your terminal in this folder and run:
    `python main_server.py`

2.  **Play the Game:**
    - Open a web browser (like Chrome or Firefox).
    - Go to the address: http://127.0.0.1:80
    - Register a new account and log in. To test multiplayer, open a second browser window (or an incognito window) and do the same with another account.

