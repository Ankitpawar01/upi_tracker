UPI Leak Detector 💳

A smart personal expense tracking and UPI spending analysis web application built with Flask and PostgreSQL.

UPI Leak Detector helps users track their expenses, understand spending patterns, import transaction statements, and identify unusual or repeated spending through automated alerts.

🚀 Features

- User Authentication: Secure signup and login.
- Expense Tracking: Add and manage transactions.
- CSV Import: Import transaction records from CSV files.
- PDF Statement Import: Extract transaction information from PDF bank statements.
- Spending Dashboard: View total spending, net worth, and top spending categories.
- Spending Analytics: Visualize spending trends and category breakdowns.
- Leak Detection Alerts: Identify repeated small expenses, frequent merchant spending, and large transactions.
- PDF Export: Generate downloadable spending reports.
- Monthly Budget: Set and monitor a monthly spending budget.
- Bank Account Tracking: View connected account information.

🛠️ Technology Stack

Technology| Purpose
Python| Backend programming
Flask| Web application framework
PostgreSQL| Database
HTML, CSS, JavaScript| Frontend
Pandas| Transaction data processing
PDFPlumber| PDF statement extraction
FPDF2| PDF report generation
Flask-Login| User authentication
Flask-Bcrypt| Password hashing
Google Gemini API| AI-assisted PDF statement extraction

📊 Dashboard

The dashboard provides:

- Total net worth
- Total spending
- Active spending alerts
- Top spending category
- Spending trend chart
- Category breakdown chart

🔍 Leak Detection

The application checks for patterns such as:

- Repeated small transactions at the same merchant.
- Frequent transactions with the same merchant.
- Large individual expenses.

These alerts help users review their spending habits. They are spending-pattern warnings, not confirmed fraud detection.

⚙️ Installation & Setup

1. Clone the repository

git clone https://github.com/Ankitpawar01/upi_tracker.git
cd upi_tracker

2. Create a virtual environment

python -m venv venv

Activate it on Windows:

venv\Scripts\activate

3. Install dependencies

python -m pip install -r requirements.txt

4. Install and configure PostgreSQL

- Install PostgreSQL.
- Start the PostgreSQL service.
- Create a database named "upi_tracker".
- Configure the database name, username, host, and password consistently in "app.py" and "init_db.py".

Important: The current public repository uses hardcoded database configuration. Replace those development values with your own local credentials before running the application. Never commit real passwords or API keys.

5. Initialize the database

python init_db.py

6. Run the application

python app.py

Open your browser:

http://127.0.0.1:5000

📂 Project Structure

upi_tracker/
│
├── app.py
├── init_db.py
├── generate_report.py
├── schema.sql
├── requirements.txt
├── Project_Report_UPI_Leak_Detector.pdf
│
├── static/
│   ├── css/
│   ├── js/
│   └── images/
│
└── templates/
    ├── dashboard.html
    ├── login.html
    ├── signup.html
    └── ...

The folders and files shown above describe the main project structure; check the repository for the complete list.

📸 Screenshots

Screenshots will be added here:

- Dashboard
- Transactions
- Spending Alerts
- CSV Upload
- PDF Export

📖 Project Report

See "Project Report – UPI Leak Detector" (Project_Report_UPI_Leak_Detector.pdf).

🔮 Future Improvements

- Improve transaction categorization.
- Add more advanced spending analytics.
- Improve security and production configuration.
- Deploy the application online.
- Add more bank statement formats and testing.

⚠️ Disclaimer

This project is intended for personal expense tracking and educational purposes. Spending alerts are based on predefined patterns and should not be treated as proof of fraudulent activity.

👨‍💻 Author

Ankit Pawar

GitHub: "Ankitpawar01" (https://github.com/Ankitpawar01)

---

⭐ If you find this project useful, consider giving the repository a star!