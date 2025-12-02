# Vision-Based-Attendence-System
🔍 Project Description

The Vision-Based Attendance System is an advanced artificial-intelligence–powered solution that uses real-time face recognition to automate the attendance process. Instead of manual attendance, the system captures faces, recognizes registered students using machine learning models, and stores attendance records in a secure database.

The system includes:

Student Registration

Face Dataset Creation

Model Training using LBPH Algorithm

Live Attendance Marking

Attendance History Viewing

Password Protection

Multiple Camera Support

Attendance Limit Control

Distance Based Face Detection & Recognition

The attendance is stored in SQLite Database with separate tables for each day.

🎯 Objective of the Project
Traditional Attendance	Vision-Based System
Time-consuming	Fast
Proxy attendance possible	Prevents impersonation
Human errors	Fully automated
Hard to store data	Easily exportable & searchable
Paper-based	Smart database logging

➡️ Provides secure, efficient, automated digital attendance suitable for universities, offices, and organizations.

🧠 Working Methodology
Step-by-Step Process
1️⃣ Register Student

User enters ID & Name via GUI

Camera captures 100–150 face images

Images stored in TrainingImage/ folder

Student details saved in StudentDetails.csv

2️⃣ Train Model

All collected images are trained using LBPH Face Recognizer

Model file stored as Trainner.yml inside TrainingImageLabel/

This is later used for prediction

3️⃣ Start Live Attendance

Webcam begins real-time face analysis

Face detected using Haarcascade Classifier

Model recognizes face from trained dataset

Name displayed on screen

Attendance logged into SQLite database with:

Name

Registration Number

Date

Time

Camera name (version 6)

4️⃣ Attendance Viewing

GUI loads table names from database

Allows user to select a date and view complete attendance list

⚙ Tools, Technologies & Libraries Used
Technology / Library	Purpose
Python	Base programming
OpenCV	Face detection & recognition, camera access
LBPH Algorithm	Machine learning model for face recognition
Haarcascade XML	Face detection
SQLite3	Attendance database
Tkinter	Graphical User Interface
PIL (Pillow)	Image preprocessing
NumPy	Image array computations
Pandas	Attendance display formatting
CV2.VideoCapture	Access webcam / IP camera
Threading (v6)	Multi-camera parallel processing
🚀 Advanced Enhancements Included
Version-wise Added Features
Version	Features Added	Improvement
v3_showAttendance.py	Dedicated window to view attendance history	Easy data retrieval
v4_range.py	Face recognition within distance range control	Better accuracy, avoids far faces
v5_limit.py	Limits attendance marking to 4 times/day	Prevents junk entries
v6_dynamic cams.py	Multiple camera support via threading + camera name logging	Supports real-world campus setups
🔐 Security Implementation

✔ Password protection for model training and admin access
✔ Change password option
✔ Prevents unauthorized modification

📦 Data Storage Format
SQLite Database Table Example
date_01_02_2025
| id | RegistrationNo | StudentName | Current_date | In_time | CameraName |

Attendance Limitation (v5/v6)

Max 4 entries per student/day in v5

Max 2 per camera in v6

📷 Camera Options
Camera Type	Support
System Webcam	Yes
IP Camera	Yes
Multiple Cameras	Yes (v6)
Real-time Threading	Yes
📈 Expected Output

Recognized student name displayed on screen

Live bounding box around face

Real-time attendance inserted to database

Interface to display attendance data

Ability to export and analyze records

🎓 Real-World Applications

Schools & Universities

Corporates & IT Companies

Hostels & Labs

Exam halls

Workforce management

Library access control

🔮 Future Enhancements
Feature	Why Needed
Deep Learning models (FaceNet, DeepFace)	More accuracy
Cloud syncing	Multiple branch campuses
Mobile App	Remote access
Offline face recognition	Low connectivity support
Mask detection	Post-COVID environments
SMS / Email notification	Automatic reporting
🧾 Conclusion

This project demonstrates a fully functional AI-based Computer Vision Attendance System integrating:

ML + GUI + DB + Image Processing + Threading

Scalable real-use functionality

High accuracy and security compared to manual attendance

It is an excellent real-world engineering project demonstrating:

Python programming

OpenCV implementation

GUI application development

SQLite database management

AI face recognition workflow
