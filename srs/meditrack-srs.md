
# MediTrack Software Requirements Specification (SRS)

## System Context

CityCare Clinic has 12 doctors, 6 receptionists, and about 400 patients per week. Appointments are currently booked by phone and paper diary, causing double bookings and long waits.

## Requirements

- **R-01** The system shall allow patients to book appointments online.
- **R-02** The system shall respond quickly to booking requests.
- **R-03** The system shall prevent double bookings.
- **R-04** Each appointment shall last 15 minutes.
- **R-05** The system shall allow doctors to set appointment length between 10 and 30 minutes.
- **R-06** The system shall send reminders to patients before appointments.
- **R-07** Patients may cancel appointments at any time and the system shall update the doctor’s schedule and notify the receptionist.
- **R-08** The system shall be user-friendly for all age groups.
- **R-09** Patient records shall be stored securely.
- **R-10** Receptionists shall be able to book appointments for walk-in patients.
- **R-11** Patients may book up to 3 active appointments.
- **R-12** The system shall be available during normal working hours.
- **R-13** Overdue payments shall be handled as per clinic policy.
- **R-14** Doctors shall be able to view their daily schedule.

## Intended Users

1. Patient
2. Doctor
3. Receptionist
4. Clinic administrator
5. Data protection officer

## Clinic Manager's Concerns

- Double bookings must never happen.
- Patients forget appointments, which costs money.
- Medical information is private.
- Elderly patients and emergency walk-ins must not be left out.
- Monday mornings are very busy.
