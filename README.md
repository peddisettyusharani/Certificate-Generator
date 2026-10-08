Certificate-Generator
A simple web-based Certificate Generator that allows users to create professional certificates by entering recipient, event, course, and date details. It provides a user-friendly interface to customize, preview, and download certificates, making it useful for academic events, workshops, competitions, training programs, and other activities.
****Certificate Generator***
## 📌 Overview

Certificate Generator is a Flask-based certificate management system that automates the creation, verification, storage, and distribution of certificates. It supports bulk certificate generation using participant data from CSV/XLSX files and generates professional PDF certificates with QR-code-based verification.

## ✨ Features

- 🔐 Admin login and authentication
- 📄 Bulk certificate generation
- 📊 Import participant details from CSV/XLSX files
- 🎨 Upload and manage custom certificate templates
- 📥 Download individual certificates
- 📦 Download multiple certificates as a ZIP file
- 🔍 Verify certificates using Certificate ID or QR code
- 📱 QR code generation for certificate verification
- 📧 Email certificates through SMTP
- 📜 Certificate generation history
- 📤 Export certificate history
- 📈 Dashboard with certificate statistics
- ⚙️ Application settings management
- 📱 Responsive user interface

## 🛠️ Technologies Used

**Backend**
- Python
- Flask
- SQLite

**Data & Document Processing**
- Pandas
- OpenPyXL
- ReportLab
- Pillow

**Additional Technologies**
- QR Code
- HTML
- CSS
- JavaScript
- Jinja2
- Python-dotenv

## 📂 Project Structure

```text
Certificate-Generation-System/
│
├── app.py
├── generator.py
├── database.py
├── config.py
├── qr_generator.py
├── email_sender.py
├── requirements.txt
│
├── templates/
├── static/
├── certificates/
├── uploads/
├── generated_zip/
├── database/
├── reports/
└── templates_certificates/
```

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd Certificate-Generation-System
```

### 2. Create a virtual environment

**Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```

**Linux/macOS:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file using `.env.example` and configure the required application and email settings.

### 5. Run the application

```bash
python app.py
```

Open the application in your browser:

```text
http://127.0.0.1:5000
```

## 🚀 How to Use

1. Login to the admin dashboard.
2. Upload participant information using CSV/XLSX.
3. Upload a certificate template if required.
4. Generate certificates in bulk.
5. Preview the generated certificates.
6. Download individual certificates or a ZIP file.
7. Use the Certificate ID or QR code to verify a certificate.
8. Send certificates through email when SMTP is configured.

## 🔎 Certificate Verification

Each generated certificate can contain a unique Certificate ID and QR code. Scanning the QR code or entering the Certificate ID allows users to verify certificate details through the verification page.

## 📊 Dashboard

The dashboard provides an overview of generated certificates and related statistics, helping administrators monitor certificate generation activity.

## 📧 Email Delivery

The system supports sending generated certificates through email using SMTP configuration. Email functionality can be enabled by adding the required SMTP credentials to the `.env` file.

## 🔒 Security

- Session-based admin authentication
- Password hashing
- Environment-based configuration
- Protected administrative functions

## 🔮 Future Enhancements

- Role-based access control
- Drag-and-drop certificate designer
- Multiple organization support
- WhatsApp certificate delivery
- Advanced certificate analytics
- Cloud deployment and storage

## 📄 License

This project is available for educational and development purposes.
