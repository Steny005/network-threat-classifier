# AI-Powered Network Threat Classification System

**Intel Unnati Industrial Training 2025**  
**Problem Statement 1: Network Security**  
**Team: Execthron**

---

## Demo Video

 [Watch Demo Video](https://drive.google.com/file/d/1SIK_kruyaB2uLdFsY7iY5bJJZ7SaKgWz/view?usp=drivesdk)

---

##  Project Overview

This project introduces a smart traffic classification system that analyzes network flow data and flags it as either **Safe** or **Malicious**.

Using a **Random Forest** model trained on the **UNSW-NB15 dataset**, it’s deployed with a simple **Flask-based web interface** where users can upload `.csv` files and view results instantly through a clean visualization.

---

##  Key Features

-  Classifies uploaded `.csv` network traffic logs in real-time.
-  Built on a trained Random Forest model.  
-  Uses **Chart.js** to display safe vs. malicious traffic visually. 
-  Flask web interface for easy user interaction. 
-  Results include only essential fields like protocol and prediction (Safe/Malicious).

---

## Dataset Used

**UNSW-NB15** – A labeled dataset containing both normal and malicious network traffic.

Included attack types:

- DoS
- Exploits  (including SQL Injection, XSS, Buffer Overflow, Shellcode, etc.)
- Fuzzers
- Reconnaissance
- Backdoors
- Analysis

> Source: [Australian Centre for Cyber Security (ACCS)](https://www.unsw.adfa.edu.au/australian-centre-for-cyber-security/cybersecurity/ADFA-NB15-Datasets/)

---

##  Tech Stack

| Layer        | Tools & Libraries                    |
| ------------ | ------------------------------------ |
| Language     | Python                               |
| Backend      | Flask, Flask-CORS                    |
| ML Libraries | Scikit-learn, Pandas, NumPy, Joblib  |
| Frontend     | HTML, CSS, JavaScript, Chart.js      |

---

## Outcomes

- Achieved **accurate classification** of malicious vs. safe traffic using a Random Forest model.
- Designed a **user-friendly interface** for uploading and analyzing `.csv` network logs.
- Successfully integrated **real-time visualization** of predictions using Chart.js.
- Demonstrated the practicality of ML models in supporting **automated network threat detection** in a lightweight environment.


---

## Limitations

- The model is trained only on **offline flow data** and does not process **live packet capture**. 
- Limited to `.csv` files with specific feature formatting; **data preprocessing must match training setup**.  
- Accuracy might vary on real-world enterprise traffic.
- No in-depth metadata like IP addresses, ports, or timestamps included.

---

##  Future Improvements

- Add support for real-time packet analysis using tools like **Scapy** or **PyShark**. 
- Include detailed traffic analytics with full metadata.
- Set up alerting systems (email, Telegram) for high-severity threats. 
- Explore deep learning models (e.g., LSTM, CNN) for better accuracy. 
- Deploy the app on the cloud and integrate with SIEM tools.

---


##  Installation Guide

### Clone the Repository

```bash
git clone https://github.com/Vasu-uu/Network-Threat-Analyzer.git
cd Network-Threat-Analyzer
```

### Install Python Packages

```bash
pip install -r requirements.txt
```

### Run the Application

```bash
python app.py
```

### Open the App

Visit in your browser:
[http://127.0.0.1:5000](http://127.0.0.1:5000)

---

---

## Contributors

* **Steny Thankkam Raju**
* **Vasudev V**
* **Jalphy Reji**

> *Submitted as part of Intel Unnati Industrial Training 2025 – Team Execthron*

---

---

## Acknowledgements

* Intel Unnati Industrial Training Team
* Australian Centre for Cyber Security - UNSW-NB15 Dataset

--- 
