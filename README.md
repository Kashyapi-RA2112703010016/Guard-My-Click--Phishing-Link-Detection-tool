GUARD MY CLICK - AI Email Scanner
GUARD MY CLICK is an advanced, automated phishing prevention tool designed to safeguard users from deceptive email scams using state-of-the-art machine learning techniques. This project leverages a combination of AI-powered algorithms and fuzzy logic to perform thorough, real-time scanning of email inboxes, identifying potential phishing attempts before they can cause harm.

🔑 Key Features
📬 Automated Inbox Scanning: Scans the user's Gmail inbox with a single click, identifying phishing threats ethically and efficiently.

🧠 Machine Learning Integration: Uses a trained ML model to analyze URLs and email metadata, offering high-accuracy phishing probability scores.

🌀 Fuzzy Logic Scoring: Evaluates URL structures with heuristic techniques to catch obfuscated and disguised phishing URLs.

⚖️ Combined Risk Analysis: Merges ML and fuzzy logic scores for robust and comprehensive threat detection.

📊 Detailed Per-URL Breakdown: Visualizes the threat level of each URL using radar charts, heatmaps, and other interactive data graphics.

📈 Interactive Dashboard: User-friendly web interface built with Bootstrap 5 and Chart.js, offering real-time scanning results and insights.

🚨 User Notifications: Real-time browser alerts and optional email notifications for detected threats.

🧾 Downloadable PDF Reports: Generate and download full scan summaries for reporting or review using jsPDF and html2canvas.

📱 Responsive Design: Modern, dark-themed UI optimized for both desktop and mobile devices.

🛠 Technologies Used
Frontend:

HTML5, CSS3 (Bootstrap 5)

JavaScript

Chart.js (visualizations)

jsPDF + html2canvas (PDF generation)

Backend:

Flask (Python Web Framework)

REST API for scan processing

Gmail API for email access

AI/ML:

Hybrid Model: Supervised Learning + Fuzzy Logic Scoring

URL-based phishing detection with feature importance scoring

Notifications:

Web Push Notifications

Email Alerts (via SMTP + secure App Passwords)

🧠 How It Works
User clicks "Start Ethical Scan".

Emails are retrieved via the Gmail API.

Each email’s URLs are extracted and analyzed using ML and fuzzy scoring.

A combined phishing risk score is computed and visualized.

Alerts are triggered if threats are detected.

Full scan results can be explored in the dashboard or exported as a PDF.

🚀 Getting Started
✅ Prerequisites
Python 3.8+

pip

Google Account with Gmail

Git installed

🔓 Setting Up Gmail API
Go to Google Cloud Console.

Create/select a project > APIs & Services > Credentials.

Click Create Credentials > OAuth client ID.

Select Desktop App, provide a name, and download the credentials.json.

Place credentials.json in the project root.

On first run, it will prompt for Gmail authentication and save token.json.

📦 Setting Up the Project
bash
Copy
Edit
# Clone the repository
git clone https://github.com/RA2112701010026/Phishing-Link-Detection-Using-a-Hybrid-ML-Fuzzy-Logic-Model-Integrated-with-Gmail-API.git

cd Phishing-Link-Detection-Using-a-Hybrid-ML-Fuzzy-Logic-Model-Integrated-with-Gmail-API

# Create virtual environment
python -m venv venv

# Activate environment
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt
🔐 Environment Variables
Create a .env file in the root directory with:

ini
Copy
Edit
SENDER_EMAIL=your_email@gmail.com
RECEIVER_EMAIL=receiver_email@gmail.com
EMAIL_PASSWORD=your_app_password
Note: If using Gmail with 2FA, generate an App Password.

🏃 Running the Application
bash
Copy
Edit
# Activate environment if not already
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Start Flask server
python app.py
Visit http://127.0.0.1:5000/ in your browser to launch the app.

👨‍💻 About Me
Name: Undekoti Rowan Ronald

Role: AI Engineer

Email: uu0712@srmist.edu.in

GitHub: [RA2112701010026](https://github.com/RA2112701010026)

LinkedIn: linkedin.com/in/undekoti-rowan-ronald
