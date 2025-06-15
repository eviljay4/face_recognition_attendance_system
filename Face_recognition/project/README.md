# face_recognition_attendance_system

A web-based attendance management system that uses **face recognition** to automate and securely record attendance. Built with **Flask**, **OpenCV**, **scikit-learn (KNN)**, and a user-friendly interface for both administrators and end users.

---

## 📸 Key Features

- ✅ Real-time face recognition using webcam
- 📅 Daily attendance log saved as `.csv`
- ➕ New user registration with automatic face dataset creation
- 🧠 Model training using K-Nearest Neighbors (KNN)
- 🌐 Web interface built with Flask and Bootstrap
- 📁 Local storage of all data (no internet required)

---

## 🛠️ Tech Stack

| Layer     | Technologies                     |
|-----------|----------------------------------|
| Backend   | Flask (Python)                   |
| Frontend  | HTML, CSS, Bootstrap, Jinja2     |
| ML Model  | OpenCV, scikit-learn (KNN), joblib |
| Storage   | CSV (attendance), local folders (faces) |

---

## 🗂️ Project Structure

project/

├── app.py # Flask application

├── haarcascade_frontalface_default.xml # Face detection model

├── templates/

│ └── home.html # Web UI template

├── static/

│ ├── background.png # UI background image (optional)

│ └── faces/ # Saved face images per user

├── Attendance/

│ └── Attendance-<date>.csv # Daily attendance logs





## 🚀 How to Run the Project

### 1. 📥 Clone the Repository

```bash
git clone https://github.com/yourusername/face-attendance-system.git
cd face-attendance-system
2. 🛠️ Install Dependencies
bash
Copy
Edit
pip install flask opencv-python scikit-learn pandas joblib
3. 🏁 Start the Application
bash
Copy
Edit
python app.py
Then open http://127.0.0.1:5000 in your browser.

📸 How It Works
Add New User

Go to the homepage

Enter a name and ID

The webcam captures 10 face images

KNN model is trained

Take Attendance

Start webcam

Recognizes and logs known faces

Data saved in Attendance/Attendance-<date>.csv

📌 Notes
Ensure haarcascade_frontalface_default.xml is in the root directory

You must register at least one user before taking attendance

Face recognition model is saved in static/face_recognition_model.pkl
