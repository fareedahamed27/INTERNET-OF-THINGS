# INTERNET-OF-THINGS
SpectraSafe: AI-Powered Anti-Piracy System for Theatres
SpectraSafe is an AI-driven, IoT-integrated solution designed to detect and disrupt mobile phone piracy in movie theatres in real time. The system combines advanced object detection, facial recognition, and infrared interference mechanisms to prevent illegal recordings while preserving the experience of genuine viewers.

Project Overview
The rise of mobile phone-based camcorder piracy has significantly impacted the film industry, leading to revenue losses and unauthorized distribution of copyrighted content. SpectraSafe tackles this issue by offering a non-intrusive, automated, and intelligent solution that operates seamlessly within cinema environments.

Key Features
Real-Time Phone Detection
Uses CCTV-like IR cameras integrated with YOLOv10s to instantly detect mobile phones aimed at the screen during screenings.

Face Recognition & Seat Mapping
Employs MTCNN for accurate facial detection and a custom grid mapping system to identify and localize the offender to a specific seat.

IR-Based Camera Disruption
Activates ESP32-controlled IR LEDs surrounding the screen to emit invisible infrared light, corrupting camera recordings without affecting human vision.

Automated Alerts
Triggers instant email notifications to theater security with face snapshots, timestamps, and seat numbers for fast response.

Real-Time Dashboard
Displays detection logs with offender details and media evidence for monitoring and future analysis.

System Architecture
Camera Input → YOLOv10s detects phone usage

Face Detection → MTCNN captures and tags offender’s face

Seat Localization → Grid mapping converts coordinates to seat number

IR Interference → ESP32 triggers IR lights to block recording

Dashboard & Alerts → Dashboard updates and emails sent instantly

Hardware & Software Stack
YOLOv10s / PyTorch – Real-time mobile phone detection

MTCNN / TensorFlow – Facial recognition

ESP32 + Arduino UNO – IoT control for IR LEDs

SQLite3 / MySQL – Detection log storage

Flask / Node.js – Backend and dashboard

SMTP / Email API – Alert distribution

IR Surveillance Cameras – Live feed for detection
