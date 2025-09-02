# Drowsiness-Detection

🚗 Drowsiness Detection System

A computer vision–based system that detects driver drowsiness in real time using OpenCV, Deep Learning, and Eye Aspect Ratio (EAR) techniques. The system alerts the driver when signs of sleepiness or eye closure are detected, helping prevent road accidents caused by fatigue.

📌 Features

Real-time face and eye detection using OpenCV.

Eye Aspect Ratio (EAR) calculation for blink & drowsiness detection.

Alarm system to alert drowsy drivers.

Supports webcam or external camera input.

Lightweight, fast, and works on CPU.

🛠️ Tech Stack

Programming Language: Python 3.x

Libraries Used:

OpenCV

dlib

imutils

playsound / winsound

NumPy

⚙️ Installation

Clone the repository:

git clone https://github.com/yourusername/drowsiness-detection.git
cd drowsiness-detection


Install dependencies:

pip install -r requirements.txt


Download the pretrained facial landmark model (shape_predictor_68_face_landmarks.dat) from dlib model download
 and place it in the project folder.

▶️ Usage

Run the script:

python drowsiness_detection.py


The system will access your webcam.

If the driver’s eyes remain closed beyond a threshold, an alarm will sound.

📊 Working Principle

Face Detection → Detect the face using dlib/OpenCV.

Eye Landmark Extraction → Extract eye regions with facial landmarks.

EAR Calculation → Compute the Eye Aspect Ratio.

Threshold Check → If EAR < threshold for consecutive frames → Drowsiness detected.

Alert System → Trigger alarm.

📷 Demo

(Add screenshots or GIFs here showing the system in action.)

🚀 Future Improvements

Add yawning detection.

Mobile integration (Android/iOS).

Advanced deep learning models (CNN, LSTMs).

Support for infrared camera for low-light environments.

📄 License

This project is licensed under the MIT License.
