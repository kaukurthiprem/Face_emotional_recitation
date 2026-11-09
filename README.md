# 🎓 Face Recognition Attendance Management System

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8-blue?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenCV-Computer%20Vision-green?logo=opencv&logoColor=white" />
  <img src="https://img.shields.io/badge/GUI-Tkinter-orange" />
  <img src="https://img.shields.io/badge/Database-MySQL-blue?logo=mysql&logoColor=white" />
</p>

<p align="center">
  <b>An Intelligent Attendance Management System Using Facial Recognition Technology</b>
</p>

---

## 👥 Team Members

**Institution:** QIS College of Engineering  
**Department:** Computer Science and Engineering  
**Academic Year:** 2025–2026

| S.No. | Team Member | Roll Number |
|---|---|---|
| 1 | T. V. Sumathi | 22491A0558 |
| 2 | M. Manvitha | 22491A0559 |
| 3 | V. Kousalya | 22491A0560 |
| 4 | Y. Likhitha | 22491A0564 |
| 5 | B. Ashok | 22491A0571 |
| 6 | **K. Prem Kumar** | **22491A0590** |

---

## 📌 Project Overview

The Face Recognition Attendance Management System is a Python-based desktop application developed using OpenCV and computer vision technology to automate student attendance.

The system captures student facial images, trains a face recognition model, identifies registered students through a webcam, and automatically records attendance.

It also provides manual attendance functionality, student management, CSV report generation, and optional database integration.

## ✨ Features

- 👤 Student Registration – Register students using their ID and name.
- 📸 Face Detection – Capture approximately 200 facial images per student.
- 🧠 Model Training – Train a face recognition model using collected images.
- ✅ Automatic Attendance – Identify registered students and record attendance.
- 📝 Manual Attendance – Mark attendance without facial recognition.
- 📊 CSV Reports – Generate attendance records based on date, time, and subject.
- 🗄️ Database Integration – Store student and attendance information using WAMP Server.
- 📷 Webcam Support – Supports default and external webcams.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python 3.8 | Core programming language |
| OpenCV | Face detection and recognition |
| Haar Cascade | Face detection |
| Tkinter | Graphical User Interface |
| Pillow (PIL) | Image processing |
| Pandas | Attendance data processing |
| CSV | Attendance report generation |
| MySQL | Database management |
| WAMP Server | Local database environment |

## 📋 Requirements

- Python 3.8
- Windows operating system
- Webcam or external camera
- Visual Studio Code / PyCharm
- WAMP Server (optional database integration)

### Install Required Libraries

```bash
pip install opencv-python
pip install Pillow
pip install pandas
```

**Note:** Tkinter is generally included with standard Python installations.

---

## 📂 Project Structure

```text
Face-Recognition-Attendance-System/
│
├── Face-Recognition-Attendance-System-main/
│   │
│   ├── TrainingImage/
│   │   └── Student Face Images
│   │
│   ├── TrainingImageLabel/
│   │   └── Trainner.yml
│   │
│   ├── StudentDetails/
│   │   └── StudentDetails.csv
│   │
│   ├── haarcascade_frontalface_alt.xml
│   ├── haarcascade_frontalface_default.xml
│   ├── training.py
│   └── testing.py
│
├── README.md
└── requirements.txt
```

## ⚙️ Installation Guide

### 1. Clone the Repository

```bash
git clone https://github.com/kaukurthiprem/Face_emotional_recitation.git
```

### 2. Navigate to the Project Directory

```bash
cd Face_emotional_recitation
```

### 3. Create a Virtual Environment

```bash
py -3.8 -m venv venv38
```

### 4. Activate the Virtual Environment

```bash
venv38\Scripts\activate
```

### 5. Install Dependencies

```bash
pip install opencv-python Pillow pandas
```

### 6. Configure Project Paths

- Create a `TrainingImage` folder if it does not exist.
- Check the image and model storage paths.
- Update file paths according to your local system.
- Ensure the webcam is connected and accessible.

## 🚀 How to Run the Project

The repository contains separate training and testing scripts.

**Run the training script:**

```bash
python training.py
```

**Run the testing script:**

```bash
python testing.py
```

Check the source code for the exact execution sequence and configuration requirements.

---

## 🔄 System Workflow

### Step 1: Student Registration

- Enter the student's ID and name.
- Click the **Take Images** button.
- The system captures approximately 200 facial images.
- Images are stored in the `TrainingImage` folder.

### Step 2: Face Recognition Training

- Click the **Train Image** button.
- The system processes the captured facial images.
- Training may take approximately 5–10 minutes for 10 persons.
- The trained model is saved in `TrainingImageLabel`.

### Step 3: Automatic Attendance

- Click the **Automatic Attendance** button.
- The webcam captures the student's face.
- The trained model identifies the registered student.
- Attendance is recorded automatically.

### Step 4: Attendance Reports

- Attendance is generated in CSV format.
- Records are organized according to date, time, and subject.
- Attendance data can also be stored in a database.

### Step 5: Manual Attendance

- Click the **Manually Fill Attendance** button.
- Enter the required attendance information.
- The system generates an attendance CSV file.
- Attendance information can also be stored in the database.

---

## 🔐 Student Login Credentials – Batch 4

The following demonstration credentials were provided with the project:

| Field | Details |
|---|---|
| Username | `batch` |
| Password | `batch4` |
| Batch | **Batch 4** |

**Note:** Change the default credentials before using the application in a real environment.

## 📷 Webcam Configuration

**Default Webcam:**

```python
cam = cv2.VideoCapture(0)
```

**External Webcam:**

```python
cam = cv2.VideoCapture(2)
```

Change the camera index according to the webcam connected to your system.

## 🗄️ Database Configuration

The application supports optional database integration using WAMP Server.

1. Install and start WAMP Server.
2. Open phpMyAdmin.
3. Create the required database.
4. Open the database configuration in the application.
5. Update the database name and connection details.
6. Run the application and verify the database connection.

## 📊 Important Project Directories

| Folder / File | Description |
|---|---|
| `TrainingImage/` | Stores captured student facial images |
| `TrainingImageLabel/` | Stores the trained recognition model |
| `StudentDetails/` | Stores student information |
| `Trainner.yml` | Trained recognition model |
| `training.py` | Model training script |
| `testing.py` | Testing and recognition script |
| `haarcascade_frontalface_default.xml` | Face detection classifier |

## 🔮 Future Enhancements

- Real-time attendance dashboard.
- Cloud-based attendance storage.
- Email and SMS notifications.
- Improved face recognition accuracy.
- Mobile application integration.
- Advanced attendance analytics.
- Export reports in Excel and PDF formats.
- Multi-camera attendance monitoring.

## 🎯 Project Outcomes

- Automated student attendance management.
- Reduced manual attendance workload.
- Faster student identification.
- Digital attendance record maintenance.
- Improved attendance management efficiency.

## 📜 License

This project was developed for educational and academic purposes as part of the B.Tech Computer Science and Engineering program at QIS College of Engineering.

## 👨‍💻 Project Author

**K. Prem Kumar**

Computer Science and Engineering  
QIS College of Engineering

- GitHub: [@kaukurthiprem](https://github.com/kaukurthiprem)
- Repository: [Face Recognition Attendance Management System](https://github.com/kaukurthiprem/Face_emotional_recitation)

---

<p align="center">
  ⭐ If you find this project useful, please give it a star on GitHub!
</p>

<p align="center">
  <b>Developed with ❤️ by K. Prem Kumar and Team</b>
</p>

<p align="center">
  Python | OpenCV | Computer Vision | Face Recognition
</p>