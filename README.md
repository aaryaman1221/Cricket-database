<img width="1470" height="956" alt="Screenshot 2025-08-20 at 12 34 36 AM" src="https://github.com/user-attachments/assets/d7656b25-8878-4eb2-b922-56ef3a7d0065" />

A web-based Cricket Database Management System built with Flask (Python), MySQL, and HTML/CSS/JS.
This project provides an admin dashboard to manage cricket data including players, teams, matches, and umpires.

📌 Features

    🔑 Login System (admin authentication)

    👨‍🏏 Player Management

    Add, edit, and delete player details

    🏏 Team Management

    ⚖️ Umpire Management

    🏟 Match Management

    📊 Dynamic tables rendered from MySQL database

🗄 Database Schema

    The database cricketwc includes:

    player – Player stats (runs, wickets, averages, etc.)

    team – Team details (batsmen, bowlers, country)

    matches – Match records with results

    umpire – Umpire info

    Additional relational tables: captain, contains, plays, played_in, umpired_by, etc.

    SQL dump is included in cricket_world_cup.sql

⚙️ Tech Stack

    Backend: Python (Flask)

Database: MySQL

Frontend: HTML, CSS, Bootstrap, Jinja2 Templates

Environment: Virtualenv

🚀 Setup Instructions
    1. Clone the repository
    git clone https://github.com/aaryaman1221/Cricket-database.git
    cd Cricket-database

    2. Create and activate virtual environment
    python3 -m venv venv
    source venv/bin/activate   # macOS/Linux
    venv\Scripts\activate      # Windows

    3. Install dependencies
    pip install -r requirements.txt

    4. Import the database

    Open MySQL and run:
    
    SOURCE cricket_world_cup.sql;

    5. Configure database connection

    Edit config.py:

    db_config = {
    "host": "localhost",
    "user": "your_mysql_username",
    "password": "your_mysql_password",
    "database": "cricketwc"
    }

    6. Run the app
    python app.py


    The app will start at:
    👉 http://127.0.0.1:3230/

    🔑 Default Admin Credentials
    Username: admin
    Password: admin


    (You can change this in app.py or use the admin table from the SQL file.)

📸 Screenshots

![Uploading Screenshot 2025-08-![Uploading Screenshot 2025-08-20 at 12.34.36 AM.png…]()
20 at 12.35.08 AM.p<img width="1470" height="956" alt="Screenshot 2025-08-20 at 12 35 25 AM" src="https://github.com/user-attachments/assets/45608bbe-98ea-433d-a9ff-0141f32db8fd" /><img width="1470" height="956" alt="Screenshot 2025-08-20 at 12 35 39 AM" src="https://github.com/user-attachments/assets/af5326c8-43c6-4dfc-8da9-23fe4e7b1718" />

ng…]()


📚 Future Improvements

    Secure authentication (hashed passwords + user roles)

    Player statistics visualization with charts

    REST API endpoints for external integration

    Enhanced frontend with React/Angular

👨‍💻 Author

Aryaman Sonawane
B.Tech Information Technology, Manipal Institute of Technology

Would you like me to also generate a requirements.txt file for your project so it works out-of-the-box on GitHub?
