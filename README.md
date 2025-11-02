🧾 Credit Card Statement Parser

A web-based Flask application that extracts and analyzes key information from multiple credit card statements (PDF format) across different banks — including HDFC, ICICI, SBI, Axis, and American Express.
It parses cardholder details, statement periods, due dates, and amounts, and generates a summary dashboard with insights and charts.

🚀 Features

Upload multiple PDF statements at once
Automatic data extraction using regex and PDF parsing
Supports multiple banks (ICICI, HDFC, SBI, AXIS, AMEX)
Visual insights dashboard with charts (Chart.js)
Download combined CSV summary of parsed results
Clean, hospital-style UI built with Bootstrap 5
Local-only processing — no data uploaded externally

🧠 Tech Stack
Layer	Technology
Backend	Python (Flask)
Frontend	HTML, CSS, Bootstrap 5, Chart.js
PDF Parsing	pdfplumber
Data Handling	pandas
Deployment	Localhost / GitHub

🧩 Project Structure
Credit-Card-Parser/
│
├── app.py                     # Main Flask application
├── templates/
│   ├── index.html             # Upload page
│   └── results.html           # Results & insights dashboard
│
├── uploads/                   # Uploaded PDF files
├── output/                    # Generated CSV output
├── venv/                      # Virtual environment (ignored in Git)
└── README.md                  # Project documentation

⚙️ Setup Instructions
1️⃣ Clone the Repository
git clone https://github.com/Yugansha-K/Credit-Card-Statement-Parser.git
cd Credit-Card-Statement-Parser

2️⃣ Create and Activate a Virtual Environment
python -m venv venv
venv\Scripts\activate     # On Windows
# or
source venv/bin/activate  # On macOS/Linux
3️⃣ Install Dependencies
pip install -r requirements.txt
If you don’t have a requirements.txt, generate one using:
pip freeze > requirements.txt
4️⃣ Run the Application
python app.py
Now open your browser and go to http://127.0.0.1:5000


🧾 How It Works
Upload multiple PDF credit card statements.
The system automatically extracts:
Cardholder name
Card last 4 digits:
Statement period
Payment due date
Total amount due
A results dashboard displays the parsed data in a table and charts.
Download all parsed results as a single CSV file.

📉 Visualization
The dashboard includes:
Bar Chart – showing total due amounts by bank
Pie Chart – showing the number of statements per bank
(Charts dynamically update based on uploaded PDFs.)

📦 Sample Use Cases
Credit card expense tracking
Financial data digitization
Multi-bank statement analytics
