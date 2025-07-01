#  Online Examination System with AI-Powered Proctoring

An end-to-end secure *Online Examination Platform* that ensures academic integrity through AI-based face recognition and behavior monitoring. The system is powered by:

- 🎓 *Django* for backend & exam management  
- 🌐 *HTML/CSS* for the frontend user interface  
- 👁 *AI Proctoring (Python)* for real-time face detection and suspicious behavior logging using *YOLOv8* and *face_recognition*

---

## ❓ Why This Project?

With the rise of remote education and online examinations, the challenge of maintaining academic honesty has become more significant. Traditional proctoring methods either:

- Are not scalable  
- Compromise privacy  
- Rely too heavily on human invigilation

*This system aims to solve that* by offering:

- 🔐 A scalable and automated way to verify user identity  
- 🛡 Real-time detection of cheating behaviors (like use of phones, additional people, or absence of the candidate)  
- ⚡ Smooth user experience for students and administrators  

---

## 🏗 Tech Stack

| Component        | Tech Used                 |
|------------------|----------------------------|
| Frontend         |  HTML, CSS                 |
| Backend          | Django (Python)            |
| Proctoring Logic | OpenCV, dlib, YOLOv8, face_recognition |
| Database         | SQLite (Django default)    |
| Deployment       | Localhost                  |



---
Built with:
- Django (Backend + HTML/CSS rendering)
- OpenCV, face_recognition, dlib (Face and behavior detection)
- YOLOv8 via Ultralytics (Object detection)

---

## 🔧 Setup Instructions
### Install dependencies 

Create virtual environment named "venv"
python -m venv venv

Activate the virtual environment
.\venv\Scripts\activate



pip install -r requirements.txt

---
### 1 Django Setup
### 🔑 Create Django Admin User

bash
py manage.py createsuperuser

### Run Django Server (Terminal 1)
bash
py manage.py makemigrations
py manage.py migrate
py manage.py runserver

---

### 2 AI Proctoring Module (Terminal 2)

bash
cd testing
python app.py


---

🚀 Features
- 🎥 Real-time webcam monitoring
- 🧠 AI-based face detection and object detection using YOLOv5
- 👥 Multiple face detection alerts
- 📵 Unauthorized object (e.g., mobile phone) detection
- ⚠️ Instant alert generation with automatic exam termination
- 🧾 Violation logging and reporting
- 🌐 Flask backend integrated with Django frontend
- 🔒 Secure role-based access for proctor and student
---

## 🛠 Common Issue Fix

If you see this error:

text
RuntimeError: Unsupported image type


Ensure your image is loaded and converted to RGB:


---

## 🙋 Contributing

Pull requests and issues are welcome! If you find a bug or have a feature request, feel free to open an issue.
