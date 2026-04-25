# Automated Employee Onboarding RPA Bot

An enterprise-grade Robotic Process Automation (RPA) solution developed for Tata Consultancy Services (TCS) to streamline the high-volume employee onboarding lifecycle.

## 🚀 Overview
The **Automated Employee Onboarding Workflow** eliminates manual document handling by orchestrating a digital pipeline that harvests candidate data from emails, validates credentials using OCR and RegEx, and synchronizes information with a central SQL database.

## 🛠 Technology Stack
* **RPA Platform:** Automation Anywhere A360
* **Database:** Microsoft SQL Server 2019
* **Scripting:** VBScript / Regular Expressions (RegEx)
* **OCR Engine:** Google Vision API
* **Communication:** IMAP/SMTP Protocols

## 📋 Key Features
* **24/7 Monitoring:** Automated harvesting of candidate documents from HR mailboxes.
* **Intelligent Extraction:** High-accuracy data capture (PAN, Aadhaar, IFSC) from PDFs and images.
* **Validation Logic:** Rule-based verification ensuring 100% data consistency.
* **Auto-Communication:** Instant delivery of personalized welcome kits and handbooks.
* **Secure Architecture:** Zero-persistence policy for PII data and encrypted credential vaulting.

## 🏗 System Architecture
The bot follows a **Dispatcher-Performer** pattern to ensure scalability:
1. **Dispatcher:** Scans the HR inbox, downloads attachments, and pushes metadata to a work queue.
2. **Performer:** Processes each candidate, performs OCR/Validation, updates the SQL DB, and triggers welcome emails.

## ⚙️ Installation & Setup
1. **Bot Agent:** Install the Automation Anywhere Bot Agent on a Windows 64-bit machine (16GB RAM recommended).
2. **Database:** Execute the SQL scripts provided in the documentation to initialize the `HR_Onboarding_DB`.
3. **Credentials:** Map `Email_Pass` and `SQL_Pass` within a secure A360 Locker named `HR_Locker`.
4. **Configuration:** Set the input/output directory paths in the bot's global variables.

## 📊 Performance Metrics
* **Turnaround Time (TAT):** Reduced by 98% (from 4 hours to <5 minutes per employee).
* **Accuracy:** 100% for digital PDFs; 94% for scanned documents with auto-routing for manual review.
* **ROI:** Achieved break-even within 4 months of deployment.

## 🔒 Security & Compliance
* **GDPR/DPDP Compliant:** Automated deletion of temporary staging files post-processing.
* **Audit Ready:** Complete timestamped logs and non-repudiation digital signatures for every database entry.

---
**Developer:** Hritik Kumar Mishra  
**Enrollment No:** 024MCA111725  
**Mentor:** Vikas Kumar Atray  
