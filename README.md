# Doctor Appointment Booking Service API

![Java](https://img.shields.io/badge/Java-8%2B-blue)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-2.5.0-green)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue)
![Maven](https://img.shields.io/badge/Maven-3.6.3-red)

This project is a Doctor Appointment Booking Service API that allows patients to schedule appointments according to their health issues.

## Framework Used

- Spring Boot

## Dependencies

The following dependencies are required to run the project:

- Spring Web
- Spring Data JPA
- MySQL Driver
- Lombok
- Validation

## Language Used

- Java

## Data Model

### Patient

- patientId
- patientName
- patientEmail
- patientPassword
- patientAge
- patientAddress
- patientGender

### Doctor

- doctorId
- doctorName
- specialization
- doctorContactNumber
- qualification
- doctorConsultationFee

### Appointment

- appointmentId
- appointmentDesc
- appointmentScheduleTime
- appointmentCreationTime

### Admin

- adminId
- adminName
- adminEmail
- adminPassword

### AuthenticationToken

- tokenId
- tokenValue
- tokenCreationDateTime

## Controllers

### PatientController API Endpoints

- POST "patient/signup"
- POST "patient/signIn"
- DELETE "patient/signOut"
- POST "appointment/schedule"
- DELETE "appointment/cancel"

### DoctorController API Endpoints

- POST "add/doctor"
- GET "doctors"

### AdminController API EndPoints

- POST "admin"
- GET "patients"
- GET "patients/Gender"
- GET "doctors/specialization"
- PUT "reschedule"

## Database Used

- SQL database
- We have used a persistent database to implement CRUD operations.

## Getting Started

- Clone this repository.
- Set up your MySQL database and update the database configuration in `application.properties`.
- Build the project using Maven: `mvn clean install`.
- Run the application: `mvn spring-boot:run`.
- Access the API using the specified endpoints.
