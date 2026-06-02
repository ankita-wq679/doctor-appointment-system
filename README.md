# doctor-appointment-system
A secure web application built with Django that automates medical scheduling, allowing patients to book dynamic time slots and doctors to manage appointments.

# Online Doctor's Appointment System 🩺
Welcome to the Online Doctor's Appointment System! This is a backend-heavy web application built using **Django** (Python framework). It is designed to solve the real-world problem of managing hospital/clinic bookings, replacing manual paperwork with a smooth digital experience.

The system manages different user roles (Patients and Doctors) and handles database relationships to prevent any double-booking issues.

 ##Tech Stack Used
* **Backend Framework:** Django (Python)
* **Database:** SQLite (Default Django database, perfect for development)
* **Frontend:** Simple HTML, CSS, and Bootstrap (for quick styling)

## Core Features

* **Dual User Portals:** Separate dashboards and login systems for both Patients and Doctors.
* **Smart Booking Logic:** Patients can filter doctors by specialization and choose an available date and time slot.
* **No Double-Booking:** The system automatically locks a time slot once a patient books it, so no two patients can book the exact same slot with the same doctor.
* **Doctor Dashboard:** Doctors can view their daily schedule, accept/cancel appointments, and manage their availability status.
* **Django Admin Panel:** Full control for the administrator to verify new doctor profiles and view overall hospital analytics.

## 🗄️ Database Structure (Models)
The project uses Django's Object-Relational Mapping (ORM) to connect four main database tables:
1. **User/Patient Model:** Stores login credentials, age, and basic medical details.
2. **Doctor Model:** Stores the doctor's name, specialization (e.g., Dentist, Cardiologist), and consultation fees.
3. **Appointment Model:** The core engine that links a Patient, a Doctor, a specific Date, and a Time Slot together.
4. **Prescription Model:** Allows doctors to add medical advice and medicine names after the check-up.

## 📁 How to Run this Project Locally

To run this Django app on your computer, you just need Python installed. Follow these quick steps:

1. Download this repository as a **ZIP** file and extract it.
2. Open your terminal/command prompt inside the extracted project folder.
3. Install Django using pip:
  
   pip install django

4. Run the database migrations to set up the tables:
 
    python manage.py migrate

5 .start the local development server:
   python manage.py runserver

6. Open your browser and go to: http://127.0.0.1:8000/

Developed as a Django backend practice project.
