# Real-Time Biometric Attendance Management System Using IoT

This project is a smart attendance system that integrates biometric fingerprint recognition with IoT technology to provide real-time, accurate, and tamper-proof attendance tracking. It is designed for educational institutions, corporate offices, and other organizations where attendance monitoring is critical.

---

## 📌 Overview

The system uses a fingerprint sensor to authenticate users and log attendance. It communicates with a web server over Wi-Fi using an ESP8266 microcontroller. Attendance records (in-time and out-time) are stored in a MySQL database and can be managed through a web-based admin dashboard.

---

## ⚙️ Technologies Used

### Hardware
- **ESP8266 NodeMCU**
- **AS608 Fingerprint Sensor**
- **0.96” OLED Display**
- **Power Supply Circuit**

### Software
- **Arduino IDE** (for embedded code)
- **PHP** (for backend logic)
- **MySQL** (for data storage)
- **HTML, CSS, JavaScript** (for dashboard UI)
- **XAMPP** (Apache + MySQL server)

---

## 🗂 Project Structure

---

## 🔐 Key Features

- **Biometric Authentication**: Secure fingerprint-based access
- **IoT Integration**: Sends data to server via HTTP over Wi-Fi
- **Real-Time Logging**: Captures in-time and out-time accurately
- **OLED Display**: Shows instant status (success/failure)
- **Web Dashboard**: Admin panel for managing users and logs
- **Database Storage**: Persistent, structured records using MySQL

---

## 🚀 Getting Started

### 1. Backend Setup
- Install [XAMPP](https://www.apachefriends.org/)
- Copy `Backend_PHP/` and `Frontend_HTML/` into `htdocs/` (e.g. `htdocs/biometricattendance`)
- Start Apache and MySQL
- Create the database using the included PHP scripts or via phpMyAdmin

### 2. Hardware & Firmware
- Open the `.ino` file in `Arduino_Code/` using Arduino IDE
- Install required libraries:
  - `Adafruit Fingerprint Sensor Library`
  - `ESP8266WiFi`, `HTTPClient`, `Adafruit_SSD1306`, `Adafruit_GFX`
- Edit Wi-Fi credentials and local IP of your backend in the code
- Upload to ESP8266 NodeMCU

### 3. Run the System
- Power the circuit (ESP8266 + Sensor + OLED)
- Scan fingerprint → sends data to server
- Data is saved to MySQL and shown on OLED
- View logs from the web dashboard

---

## 🔧 Folder Highlights

- `Arduino_Code/biometric_attendance.ino`: Handles fingerprint detection and server communication
- `Backend_PHP/`: Creates and connects to the database, processes attendance
- `Frontend_HTML/`: Displays attendance logs to the admin
- `project_report.pdf`: Explains the project in detail with code and circuits

---

## 🔭 Future Improvements

- Add mobile app interface
- Use cloud-based storage (e.g., Firebase or AWS)
- Add support for facial or voice recognition
- Generate automated reports (PDF/Excel export)
- Power optimization for portable versions

---

## 📄 License

This project is provided for educational and research purposes only. Use or modify it at your own discretion.


