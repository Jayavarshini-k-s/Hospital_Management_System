# 🏥Hospital_Management_System
 The Hospital Management System (HMS) is a Java Swing + Oracle SQL-based desktop application designed to help hospitals efficiently manage patients, doctors, rooms, and appointments in a structured and user-friendly way. It allows hospital staff to insert, delete, and update patient records, manage doctor and room details, and maintain organized hospital data securely in an Oracle database, ensuring quick access and easy modifications of records whenever needed.

---

## ✨ Features

* **Login System** allowing staff/admin to log in securely.
* **Dashboard** with:

  * Patient Management
  * Doctor Management
  * Room Management
  * Appointment Management
* **Patient Management**:

  * Insert new patient details (`PatientID`, `PatientName`, `DateOfBirth`, `Gender`).
  * Delete patient by `PatientID`.
  * Update patient details by `PatientID`.
* **Doctor Management**:

  * Insert, delete, and update doctor details (`DoctorID`, `DoctorName`, `Specialization`, `PhoneNumber`, etc.).
* **Room Management**:

  * Insert, delete, and update room details (`RoomID`, `Patient_ID`, `RoomType`, `BedCount`, etc.).
* **User-friendly GUI** using Java Swing:

  * Easy navigation between modules.
  * Clear success/error dialogs for operations.
* **Database**:

  * Uses **Oracle SQL** for persistent storage.
  * Ensures data consistency and retrieval for each module.

---

## 🛠️ Tech Stack

* **Java (Swing)**: GUI development.
* **Oracle SQL**: Database operations.
* **JDBC**: Database connectivity.

## 🛠️ Tool
* Netbeans
---

## 🚀 Setup Instructions

### 1️⃣ Clone this repository

```bash
git clone https://github.com/yourusername/HospitalManagementSystem.git
cd HospitalManagementSystem
```

### 2️⃣ Set up Oracle Database

* Create tables:

  * `Patients`
  * `Doctors`
  * `Rooms`
  * `Appointments`

### 3️⃣ Configure Database Credentials

* In Java files, set your Oracle DB `username`, `password`, and connection URL:

  ```java
  DriverManager.getConnection("jdbc:oracle:thin:@localhost:1521:XE", "username", "password");
  ```
* Ensure Oracle listener is running.

### 4️⃣ Add Oracle JDBC Driver

* Download `ojdbc8.jar`.
* Add to your IDE libraries or CLI classpath.

### 5️⃣ Run the Application

* Compile and run `MainFrame.java`.
* Navigate to **Patient**, **Doctor**, **Room**, and **Appointment** management modules.

---

## 📂 Project Structure

```plaintext
HospitalManagementSystem/
│
├── src/
│   ├── MainFrame.java
│   ├── DashboardFrame.java
│   ├── PatientOperationFrame.java
│   ├── InsertPatientFrame.java
│   ├── DeletePatientFrame.java
│   ├── UpdatePatientFrame.java
│   └── ...
│
├── sql_scripts/
│   ├── create_tables.sql
│   └── insert_sample_data.sql
│
├── README.md
└── LICENSE
```

---

## 📸 Screenshots

### Login Page
<p align="center">
  <img src="https://github.com/user-attachments/assets/208aded3-b932-4382-9ee0-a7a72b895e39" alt="Hospital Management System Screenshot" width="500">
</p>

### Dashboard 
<p align="center">
  <img src="https://github.com/user-attachments/assets/5c0bb3c9-4c57-4d5d-ae13-b2be655c355c" alt="Hospital Management System Screenshot" width="500">
</p>
---

## 📌 Description

The **Hospital Management System** helps hospital staff efficiently manage patient, doctor, room, and appointment data with an intuitive Java Swing GUI and persistent Oracle SQL backend.

---

