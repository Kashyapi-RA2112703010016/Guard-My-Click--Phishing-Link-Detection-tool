**Project Description: GUARD MY CLICK - AI Email Scanner**

GUARD MY CLICK is an advanced, automated phishing prevention tool designed to safeguard users from deceptive email scams using state-of-the-art machine learning techniques. This project leverages a combination of AI-powered algorithms and fuzzy logic to perform thorough, real-time scanning of email inboxes, identifying potential phishing attempts before they can cause harm.

**Key Features**

Automated Inbox Scanning: The system performs an ethical scan of the user's email inbox with a single click, analyzing each email for phishing risks.

Machine Learning Integration: Utilizes a trained machine learning model that evaluates URLs and email metadata to assign a phishing probability score, improving detection accuracy beyond traditional rule-based methods.

Fuzzy Logic Scoring: Complements ML predictions by assessing URLs with fuzzy risk scoring techniques to capture obfuscated phishing attempts.

Combined Risk Analysis: Merges ML and fuzzy scores to provide a comprehensive risk assessment, improving the reliability of phishing detection.

Detailed Per-URL Breakdown: Presents a granular analysis for every suspicious URL with visualizations such as radar charts and heatmaps showing feature importance and risk factors.

Interactive Dashboard: Displays scan results in a user-friendly interface, including summary tables, alert modals, and graphical insights using Chart.js.

User Notifications: Supports desktop browser notifications and email alerts to immediately inform users of detected phishing threats.

Downloadable PDF Reports: Users can export detailed scan summaries and risk analyses in PDF format for record-keeping or further review.

Responsive Design: Built with Bootstrap and a dark theme to ensure accessibility and modern UI experience on all devices.

**Technologies Used**

Frontend: HTML5, CSS3 (Bootstrap 5), JavaScript, Chart.js for data visualization, jspdf and html2canvas for PDF generation.

Backend (implied): Likely a REST API that processes scan requests and returns JSON-formatted phishing analysis results.

Machine Learning Model: A custom phishing detection model combining supervised learning classifiers and heuristic scoring.

Notification System: Web Push Notifications and Email API integration for timely alerts.

Security Focus: Ethical scanning practices ensure privacy and data security during email analysis.

**How It Works**

User initiates scan by clicking the "Start Ethical Scan" button.

The frontend calls a backend /scan endpoint that fetches emails and analyzes each message.

URLs extracted from emails undergo machine learning evaluation and fuzzy scoring.

Results, including phishing likelihood and feature importance, are returned and displayed.

If phishing emails are detected, the user receives alerts via modal popups, browser notifications, and optional email notifications.

Users can explore detailed URL-level analysis with interactive charts and export the full report as a PDF.



## Getting Started

### Prerequisites

- Python 3.8 or higher
- A Google account to set up Gmail API access
- `pip` package manager

---

### Setting Up Gmail API Credentials

1. Go to the [Google Cloud Console](https://console.cloud.google.com/).
2. Create a new project or select an existing one.
3. Navigate to **APIs & Services > Credentials**.
4. Click **Create Credentials > OAuth client ID**.
5. Choose **Desktop app** and give it a name.
6. Download the `credentials.json` file.
7. Place `credentials.json` in your project root directory.

The first time you run the app, it will prompt you to authorize access to your Gmail account. After authorization, a `token.json` file will be saved locally to maintain authentication.

---

### Setting Up the Virtual Environment

1. Open a terminal/command prompt in your project folder.
2. Create a virtual environment:

   ```bash
   python -m venv venv
Activate the virtual environment:

On Windows:

venv\Scripts\activate
On macOS/Linux:

source venv/bin/activate

Installing Dependencies
Install all required packages using requirements.txt:

pip install -r requirements.txt

Setting Environment Variables
Create a .env file in your project root with the following variables:

SENDER_EMAIL=your_email@gmail.com
RECEIVER_EMAIL=receiver_email@gmail.com
EMAIL_PASSWORD=your_email_app_password
Note: For EMAIL_PASSWORD, you may need to create an App Password if you use Gmail with 2FA enabled.

Running the Application
Activate the virtual environment (if not already active).

Run the Flask app:
python app.py
Open your browser and visit:
http://127.0.0.1:5000/
