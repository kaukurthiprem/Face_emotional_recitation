# 🎓 Face Recognition Attendance Management System

An automated **Attendance Management System** built using **Python and OpenCV** that identifies registered students through facial recognition and records their attendance automatically.

The system provides an easy-to-use GUI for student registration, face image collection, model training, automatic attendance, and manual attendance management.

---

## ✨ Features

- 👤 **Student Registration** – Register students using their ID and name.
- 📸 **Face Detection & Image Collection** – Capture up to 200 face images per student.
- 🧠 **Face Recognition Training** – Train the recognition model using collected face images.
- ✅ **Automatic Attendance** – Recognize students and record attendance automatically.
- 📝 **Manual Attendance** – Mark attendance manually without facial recognition.
- 📊 **CSV Attendance Reports** – Generate attendance records based on date, time, and subject.
- 🗄️ **Database Integration** – Store student and attendance information using WAMP Server.
- 📷 **Webcam Support** – Supports both default and external webcams.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python 3.8 | Core programming language |
| OpenCV | Face detection and recognition |
| Tkinter | Graphical User Interface |
| Pillow (PIL) | Image processing |
| Pandas | Attendance data management |
| CSV | Attendance record storage |
| WAMP Server | Database integration |

## 📋 Requirements

Install the following dependencies:

```bash
pip install opencv-python
pip install Pillow
pip install pandas
```

**Note:** Tkinter is included with most standard Windows Python installations.

## 📁 Project Setup

### 1. Clone the repository

```bash
git clone https://github.com/kaukurthiprem/Face_emotional_recitation.git
```

### 2. Navigate to the project folder

```bash
cd Face_emotional_recitation
```

### 3. Create a Python virtual environment

```bash
py -3.8 -m venv venv38
```

### 4. Activate the virtual environment

```bash
venv38\Scripts\activate
```

### 5. Install the required libraries

```bash
pip install opencv-python Pillow pandas
```

### 6. Configure project paths

- Create a `TrainingImage` folder in the project directory if it does not already exist.
- Open `AMS_Run.py`.
- Update all file paths according to your local system directory.

## 🚀 How to Run the Project

Execute the following command:

```bash
python AMS_Run.py
```

## ⚙️ How the System Works

### Step 1: Student Registration

- Enter the student's ID and name in the application.
- Click the **Take Images** button.
- The system captures approximately 200 face images.
- Captured images are stored in the `TrainingImage` folder.

### Step 2: Train the Recognition Model

- Click the **Train Image** button.
- The system processes the collected face images.
- Training may take approximately 5–10 minutes for 10 persons.
- The trained model is saved in `TrainingImageLabel`.

### Step 3: Automatic Attendance

- Click the **Automatic Attendance** button.
- The webcam captures the student's face.
- The trained model identifies the registered student.
- Attendance is recorded automatically.

### Step 4: Attendance Reports

- Attendance records are generated in CSV format.
- Records are organized according to time and subject.
- Attendance data can also be stored in a database.

### Step 5: Manual Attendance

- Click the **Manually Fill Attendance** button.
- Enter attendance details manually.
- The system generates a CSV attendance file and can store records in the database.

## 🗄️ Database Configuration

To enable database integration:

1. Install and configure WAMP Server.
2. Create your database.
3. Open `AMS_Run.py`.
4. Update the database name and connection details according to your configuration.

## 📷 Webcam Configuration

**Default webcam:**

```python
cam = cv2.VideoCapture(0)
```

**External webcam (if detected as camera index 2):**

```python
cam = cv2.VideoCapture(2)
```

If your webcam is not working, try changing the camera index.

## 🔐 Student Login Details

The following credentials are provided in the project configuration:

| Field | Value |
|---|---|
| Username | `batch` |
| Password | `batch4` |

*These are the supplied demonstration credentials. Change them before deploying the application or publishing real student data.*

## 📂 Important Project Folders

| Folder / File | Description |
|---|---|
| `TrainingImage/` | Stores captured student face images |
| `TrainingImageLabel/` | Stores the trained recognition model |
| `StudentDetails/` | Stores student information |
| `AMS_Run.py` | Main application entry point, as described in the setup instructions |

## 🔮 Future Improvements

- Cloud-based attendance storage.
- Real-time attendance dashboard.
- Improved face recognition accuracy.
- Email notifications for attendance.
- Export attendance reports in Excel and PDF formats.

## 👨‍💻 Author

**Kasukurthi Prem Kumar**

- GitHub: [@kaukurthiprem](https://github.com/kaukurthiprem)

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub!

---

**Built with ❤️ using Python and OpenCV.**