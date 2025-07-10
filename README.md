# FUTURE_CS_03

## 🚩 Task 3 — Secure File Sharing System

This repository contains my completed work for Task 3 of the Future Interns Cyber Security Internship.

---

### 📌 What it does

- Uses Flask and AES encryption (PyCryptodome) to securely upload and share files.
- POST `/upload`: Uploads a file, encrypts it with AES, saves it as `.enc`.
- GET `/download/<filename>`: Decrypts the `.enc` file and returns the original securely.

---

### 📌 How to run

1. Clone this repo:
   git clone https://github.com/Sagar-Ez/FUTURE_CS_03.git
   cd FUTURE_CS_03

2. Create a virtual environment:
   python3 -m venv venv
   source venv/bin/activate

3. Install dependencies:
   pip install Flask pycryptodome

4. Run the Flask app:
   python app.py

5. Use Postman to test:
   - POST `/upload` → Upload a file.
   - GET `/download/<filename>` → Download the decrypted file.

---

### 📸 Proof

The `screenshots/` folder shows:
- Successful upload with encryption (`test.txt.enc`)
- Successful download with decryption (`decrypted_test.txt`)
- The `uploads/` folder with both files
### 📸 Screenshots

1️⃣ POST upload success — ![POST Upload](screenshots/postman_upload.png)  
2️⃣ GET download success — ![GET Download](screenshots/postman_download.png)  
3️⃣ `uploads/` folder with encrypted & decrypted files — ![Uploads Folder](screenshots/uploads_folder.png)

---

✅ Task 3 completed and verified.
