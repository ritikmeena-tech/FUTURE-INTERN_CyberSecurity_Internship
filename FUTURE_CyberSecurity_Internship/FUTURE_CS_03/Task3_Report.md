
# 🔐 Secure File Sharing System – Report (Task 3)

**Intern:** Ritik Meena  
**Internship Track:** Cyber Security  
**Task:** Task 3 – Secure File Sharing System  
**Tools Used:** Python Flask, PyCryptodome, Postman, curl

---

## 📌 Objective
Build a secure file upload/download portal using AES encryption to protect files at rest and during transmission.

---

## ⚙️ Tools & Technologies
- **Python Flask:** Backend web application
- **PyCryptodome:** AES encryption in EAX mode
- **Postman/curl:** API interaction and testing

---

## 🔒 Security Architecture
- Files are encrypted using AES-128 immediately upon upload.
- Encrypted files are stored on the server.
- Files are decrypted only temporarily during download and served securely.
- Key is stored in memory (can be replaced with secure key storage in production).
- Communication over HTTP for testing; HTTPS recommended in production.

---

## 🚀 How to Use

1. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```

2. Start the server:
   ```bash
   python app.py
   ```

3. Upload a file:
   ```bash
   curl -F "file=@yourfile.txt" http://127.0.0.1:5000/upload
   ```

4. Download the file:
   ```bash
   curl -O http://127.0.0.1:5000/download/yourfile.txt
   ```

---

## 📄 Files Delivered

| File | Description |
|------|-------------|
| `app.py` | Flask backend for encryption and API routes |
| `requirements.txt` | Python dependencies |
| `SECURITY_OVERVIEW.md` | Security design summary |
| `README.md` | Task overview and run instructions |

---

## 🧠 Key Learnings

- Implemented secure file encryption using AES
- Developed a functioning Flask-based file API
- Understood the importance of secure file handling in web applications

---

**Submitted by:** Ritik Meena  
**Internship:** Future Interns Cyber Security – July 2025
