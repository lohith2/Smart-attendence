🧠Smart Attendance using Facial Recognition 

An intelligent Face Recognition–Based Attendance System built with Python and OpenCV. This system automates attendance marking by detecting and recognizing faces of registered students in real time, improving accuracy and eliminating manual errors.

---

🚀 Features

- 🎥 Real-time face detection and recognition using OpenCV and Haar Cascade Classifier  
- 🧑‍🎓 Student registration and dataset creation
- 📋 Automatic attendance logging (CSV-based or database-ready)  
- ⚡ Fast and lightweight, suitable for classroom or office environments  
- 🔐 Secure and unique identification based on facial features  

---

🧰 Tech Stack

- Language: Python 3.x  
- Libraries: OpenCV, NumPy, Pandas (optional), CSV  
- Model: Haar Cascade Classifier (`haarcascade_frontalface_default.xml`)  
- Storage: CSV file (`StudentDetails/StudentDetails.csv`)  

---

⚙️ Installation

1. Clone the repository**
   ```bash
   git clone https://github.com/yourusername/Smart-attendence.git
   cd Smart-attendence-master
   ```

2. Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
   *(If `requirements.txt` isn’t present, manually install the main dependencies below)*  
   ```bash
   pip install opencv-python numpy pandas
   ```

3. Ensure Haar Cascade is available
   The project already includes `haarcascade_frontalface_default.xml`.  

---

🧠 Usage

1. Train the model
   ```bash
   python train.py
   ```

2. Run the attendance system
   ```bash
   python setup.py
   ```

3. View Attendance
   Check the generated CSV file:
   ```
   StudentDetails/StudentDetails.csv
   ```

---

📁 Folder Structure

```
Smart-attendence-master/
│
├── setup.py                  # Main attendance script
├── train.py                  # Model training script
├── haarcascade_frontalface_default.xml  # Face detection model
├── StudentDetails/            # Stored student data and attendance logs
│   └── StudentDetails.csv
└── README.md
```

---

🧑‍💻 How It Works

1. Face Detection: Uses Haar Cascade to detect faces from webcam input.  
2. Training: Captured faces are stored, then used to train a face recognizer model.  
3. Recognition: When a known face is detected, attendance is logged automatically in a CSV file.  

