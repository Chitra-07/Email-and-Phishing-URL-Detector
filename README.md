# 🛡️ Email & Phishing URL Detector

A full-stack cybersecurity web application that helps users validate email addresses and identify phishing URLs through rule-based security analysis. The application provides real-time risk assessment, security recommendations, and phishing detection using a React frontend and Flask backend.

---

## ✨ Features

### 📧 Email Validation
- Validates email format using Regular Expressions (Regex)
- Detects known phishing email domains
- Identifies disposable email providers
- Verifies DNS MX records
- Calculates email security score (0–100)
- Provides personalized security recommendations
- Displays similar email addresses from previous analyses

### 🔗 Phishing URL Detection
- Detects known phishing domains
- Identifies suspicious Top-Level Domains (TLDs)
- Detects typosquatting attempts
- Detects IP-based URLs
- Detects excessive subdomains
- Analyzes phishing-related keywords
- Generates phishing risk score with warnings

### 📊 Additional Features
- RESTful API architecture
- JSON-based data storage
- Security score analysis
- Statistics endpoint
- Health check endpoint
- Responsive React user interface

---

# 🛠️ Tech Stack

## Frontend
- React.js
- JavaScript
- HTML5
- CSS3

## Backend
- Python
- Flask
- Flask-CORS

## Libraries
- dnspython
- urllib.parse
- Regular Expressions (re)

## Storage
- JSON Files

---

# 📁 Project Structure

```text
Email-and-Phishing-URL-Detector
│
├── backend
│   ├── app.py
│   ├── email_validator.py
│   ├── phishing_detector.py
│   ├── requirements.txt
│   └── data
│       ├── email_analyses.json
│       └── phishing_urls.json
│
├── frontend
│   ├── public
│   ├── src
│   │   ├── components
│   │   ├── App.js
│   │   └── index.js
│   ├── package.json
│   └── package-lock.json
│
├── .gitignore
└── README.md
```

---

# ⚙️ How It Works

## Email Validation

1. User enters an email address.
2. The React frontend sends the request to the Flask backend.
3. The backend:
   - Validates email format
   - Verifies email domain
   - Detects phishing and disposable domains
   - Checks DNS MX records
   - Calculates a security score
4. Results and recommendations are displayed to the user.

---

## Phishing URL Detection

1. User enters a URL.
2. The backend analyzes:
   - Known phishing domains
   - Suspicious domain extensions
   - Typosquatting attempts
   - IP-based URLs
   - Excessive subdomains
   - Phishing keywords
3. A phishing risk score and security warnings are returned.

---

# 🚀 Installation

## Prerequisites

Make sure the following are installed:

- Git
- Python 3.10 or later
- Node.js (LTS recommended)
- npm

---

## Clone the Repository

```bash
git clone https://github.com/Chitra-07/Email-and-Phishing-URL-Detector.git
cd Email-and-Phishing-URL-Detector
```

---

## Backend Setup

```bash
cd backend
pip install -r requirements.txt
python app.py
```

The Flask backend will start on:

```text
http://localhost:5000
```

---

## Frontend Setup

Open a **new terminal** and run:

```bash
cd frontend
npm install
npm start
```

The React application will start on:

```text
http://localhost:3000
```

Open your browser and visit:

```text
http://localhost:3000
```

---

# 📡 API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | `/api/validate-email` | Validate an email address |
| POST | `/api/detect-phishing` | Detect phishing URLs |
| GET | `/api/security-score/<email>` | Get detailed email security analysis |
| GET | `/api/similar-emails/<email>` | Retrieve similar email addresses |
| GET | `/api/stats` | View application statistics |
| GET | `/api/health` | Check backend health status |

---

# 🔒 Security Checks Performed

### Email Validation
- Regex validation
- Trusted domain verification
- Disposable email detection
- Phishing domain detection
- DNS MX record verification

### URL Detection
- Known phishing domain detection
- Suspicious TLD detection
- Typosquatting detection
- IP-based URL detection
- Excessive subdomain detection
- Keyword-based phishing analysis

---

# 📈 Future Enhancements

- Integrate machine learning models for phishing prediction
- Replace JSON storage with MongoDB or MySQL
- User authentication and authorization
- Email attachment scanning
- Real-time threat intelligence integration
- Analytics dashboard
- Deploy the application online

---

# 👩‍💻 Author

**D Chitra**

GitHub: https://github.com/Chitra-07

---

## ⭐ If you found this project useful, consider giving it a star!
