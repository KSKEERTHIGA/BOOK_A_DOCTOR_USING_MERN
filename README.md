# BOOK_A_DOCTOR_USING_MERN
The "Booking a Doctor's Appointment System Using MERN Stack" project
aims to develop a web application that simplies the process of scheduling medical
appointments. Leveraging the MERN stack (MongoDB, Express.js, React, and
Node.js), this application provides a seamless and ecient platform for patients and
healthcare providers.

---
## Table of Contents

- [Features](#features)
- [System Requirements](#system-requirements)
- [Project Architecture](#project-architecture)
- [Installation and Setup](#installation-and-setup)
- [Environment Variables](#environment-variables)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)
- [Project Implementation & Execution](#project-implementation--execution)

- ---
## Features
- **User Registration & Authentication**: Supports roles for Patients and Doctors with secure access.
- **Doctor Listings**: Doctors can manage their profiles with specialization, fees, and availability.
- **Doctor Search & Filters**: Patients can search by specialization, location, fees, and availability.
- **Appointment Booking**: Patients book appointments; doctors confirm or decline.
- **Admin Role**: Admin reviews doctor registrations, monitors activity, and governs the platform.
- **Real-Time Updates**: Instant updates for appointment confirmations, cancellations, and rescheduling.
---

## System Requirements
- **Hardware**: Windows 8 or higher machine with a stable internet connection (30 Mbps recommended).
- **Software**: Node.js, MongoDB, React, Express.js, and two web browsers (for testing).
  
  ---
## Project Architecture

This project follows a client-server architecture:

- **Frontend**: Built with React and styled using Bootstrap or Material UI for a user-friendly and responsive interface.
- **Backend**: Developed with Express.js, managing API requests and connecting to MongoDB for seamless data flow.
- **Database**: MongoDB stores user accounts, doctor profiles, and appointment information.
  
  ---
  ## Installation and Setup

### Prerequisites

1. **Node.js & npm**: Install [Node.js](https://nodejs.org/en/download/).
2. **MongoDB**: Install [MongoDB](https://www.mongodb.com/try/download/community).

### Step-by-Step Guide
1. **Clone the Repository**:
   ```bash
     git clone https://github.com/your-username/book-a-doctor.git  
     cd book-a-doctor  
   ```

2. **Backend Setup**:
   - Navigate to the backend folder:
     ```bash
     cd backend
     ```
   - Install dependencies:
     ```bash
     npm install
     ```
   - Create an `.env` file in the `backend` directory (see Environment Variables section below).
   - Start the backend server:
     ```bash
     npm start
     ```

3. **Frontend Setup**:
   - Open a new terminal and navigate to the frontend folder:
     ```bash
     cd frontend
     ```
   - Install dependencies:
     ```bash
     npm install
     ```
   - Start the frontend server:
     ```bash
     npm start
     ```

4. **Access the App**:
   - Open your browser and go to `http://localhost:3000` for the frontend and `http://localhost:8000` for the backend.

---

## Environment Variables

Create an `.env` file in the `backend` directory and configure the following environment variables:

```plaintext
PORT=8000
MONGO_URI=your_mongodb_connection_string
JWT_KEY= cVjH7n6M4pZ1jK2dN8oX1bXrQw2+Jk8Gx5zS1R3iZ+fVjFcQ0AhVFnQYmK5e25a
```

- **PORT**: Port number for backend server (default is 8000).
- **MONGO_URI**: MongoDB connection string.
- **JWT_KEY**: Secret key for JSON Web Token (JWT) authentication.

---

## Usage

### Roles and Functionality

1. **Patient**: Registers, searches for doctors, books appointments, and tracks appointment status.
2. **Doctor**: Registers and awaits admin approval, updates profile, manages schedule, and handles appointment requests.
3. **Admin**: Approves doctor registrations, manages user activity, and enforces platform policies.
   
### Typical User Flow

- **Patient**: Registers/logs in, searches for doctors, books an appointment, and receives confirmation or rescheduling details.
- **Doctor**: Registers/logs in, updates availability, and confirms or declines appointments.
- **Admin**: Reviews and approves doctor accounts, monitors activities, and ensures platform compliance.

  ---
## Folder Structure

```plaintext
Book-a-doctor/
frontend/                    # React frontend
├── public/                  # Public assets
├── src/                     # Source files
│   ├── components/          # Component directory
│   │   ├── admin/           # Admin-specific components
│   │   │   ├── AdminApproval.jsx
│   │   │   ├── AdminDashboard.jsx
│   │   │   ├── AdminHome.jsx
│   │   │   └── AdminUsers.jsx
│   │   ├── common/          # Common components
│   │   │   ├── Home.jsx
│   │   │   ├── Login.jsx
│   │   │   ├── Notification.jsx
│   │   │   └── Register.jsx
│   │   ├── user/            # User-specific components
│   │       ├── AddDoctor.jsx
│   │       ├── ApplyDoctor.jsx
│   │       ├── DoctorList.jsx
│   │       ├── UserAppointments.jsx
│   │       └── UserHome.jsx
│   ├── images/              # Images directory
│       ├── p2.png
│       ├── p3.webp
│       └── photo1.png
├── App.css                  # CSS file for the application
├── App.js                   # Main application component
├── index.js                 # React DOM rendering entry point
.gitignore                   # Files to ignore in version control
package-lock.json            # Exact versions of installed dependencies
package.json                 # Application metadata and dependencies
```

---
## Contributing

Contributions are welcome! Please follow these steps:

1. Fork this repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

---
## Project Implementation & Execution

Once development is complete, the application is tested to ensure all features are functional and bug-free. The following are screenshots of the key components of the app:

- **Landing Page**:
  
    ![Landing Page](https://github.com/user-attachments/assets/ded750b8-daf7-4369-befe-3857abfa3d82)

- **Register Page and Login**:

    ![Register Page](https://github.com/user-attachments/assets/ba7bbaa7-685c-4cad-89e3-d5dffe8b300f)

    ![Login Page](https://github.com/user-attachments/assets/95607082-6c41-441c-8791-7d8507a2811f)

- **Admin Dashboard**:

    ![Admin Dashboard](https://github.com/user-attachments/assets/c3b06ba6-e283-4c41-9f70-4545bb831f66)

- **Doctor Dashboard**:
  
    ![Doctor Dashboard](https://github.com/user-attachments/assets/082c1831-8bf4-48eb-a33f-6fd54f1a8e20)

- **User Dashboard**:

    ![User Dashboard](https://github.com/user-attachments/assets/653fab2d-6f99-47c8-af14-4b5e01bbccd1)

---


