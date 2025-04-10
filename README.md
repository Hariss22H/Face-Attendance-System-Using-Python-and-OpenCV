# 🎓 FaceProof: AI-Powered Face Recognition Attendance System

A robust, real-time face recognition attendance system built with OpenCV, Python, and Tkinter. Designed to automate attendance tracking in educational institutions, FaceProof ensures accuracy, efficiency, and zero contact interaction—suitable for the modern, post-pandemic world.

---

## 🚀 Features

- 🔍 **Face Registration** – Capture and register student images with Enrollment Number & Name.
- 🧠 **Model Training** – Train LBPH (Local Binary Pattern Histogram) recognizer on collected images.
- 🕵️‍♂️ **Real-time Face Detection & Recognition** – Uses Haar cascade for face detection and LBPH for recognition.
- 📊 **Attendance Logging** – Logs timestamped attendance with subject name and auto-generates CSV files.
- 📁 **Excel Export & CSV Viewer** – View and export attendance records with a simple GUI.
- 🔊 **Text-to-Speech Feedback** – System voice guides the user during operations.
- 🎨 **User Interface** – Intuitive Tkinter GUI with themed visual buttons and icons.

---

## 📁 Project Structure
```
Project_FaceAttendance/
│
├── haarcascade_frontalface_alt.xml        # Haar cascade classifier for face detection
├── attendance.py                          # Main GUI launcher
├── automaticAttedance.py                  # Real-time attendance marking module
├── takeImage.py                           # Module to capture and save student face images
├── trainImage.py                          # Module to train LBPH model using captured images
├── show_attendance.py                     # Module to display saved attendance records
│
├── StudentDetails/                        # CSV file storing student names & enrollment IDs
│   └── studentdetails.csv
│
├── TrainingImage/                         # Captured face images organized per student
│
├── TrainingImageLabel/
│   └── Trainner.yml                       # Trained LBPH face recognition model
│
├── Attendance/                            # Auto-generated attendance CSV files (per subject/date)
│
└── UI_Image/                              # Icons and button images used in the UI
    ├── 0001.png
    ├── register.png
    ├── attendance.png
    └── verifyy.png
```

---

## 🛠️ Requirements

- Python 3.6+
- OpenCV  
- Tkinter (built-in)  
- Pillow  
- Pandas  
- NumPy  

> Install using:  
```bash
pip install opencv-python pillow pandas numpy
```

---
## 💡 How It Works

### 📸 Register Faces
Enter student details → Capture 60 face samples per student → Save them for training.

### 🧠 Train Model
Train the **LBPH (Local Binary Pattern Histogram)** face recognizer using the captured images.

### 🎯 Take Attendance
Start webcam → System detects & recognizes faces → Compares with trained model → Marks students as 'Present' for the selected subject.

### 📊 View Attendance
Browse attendance logs stored by subject & date → Export as CSV files for reporting or analysis.
---
## 📌 Limitations
-Sensitive to lighting and face orientation.

-Requires decent hardware (8 GB RAM & GPU recommended) for smooth real-time processing.

---

## 📸 Screenshots

--
## 🙋‍♂️ Author

**Shaik Harriss Razvi**  
Student @ Alliance University  
Machine Learning & OpenCV Enthusiast  

🔗 [LinkedIn](https://www.linkedin.com/in/hariss-razvi-shaik-31b037333/) | [GitHub](https://github.com/Hariss22H)

