# MediTrack Validation Findings

## Summary

The review identifies major gaps and one direct contradiction in the supplied SRS. The document should be revised before the clinic approves the contract.

## Findings

| ID | Related requirement(s) | Finding | Impact / Risk | Recommended Clarification |
|---|---|---|---|---|
| F-01 | R-04, R-05 | Appointment duration is contradictory: R-04 fixes appointments at 15 minutes, while R-05 allows doctors to select 10–30 minutes. | Incorrect schedules and inconsistent booking behaviour. | State whether 15 minutes is the default or fixed duration, and define who may change it and within what limits. |
| F-02 | R-02 | "Respond quickly" is not measurable. | Performance cannot be objectively tested, especially during busy periods. | Specify a response-time target, unit, and expected load. |
| F-03 | R-03 | Double-booking prevention has no measurable acceptance criteria. | Two patients may receive the same doctor's time slot. | Define conflict handling for simultaneous requests and require that a doctor/time slot cannot be confirmed twice. |
| F-04 | R-06 | Reminder lead time and delivery channel are missing. | Patients may still forget appointments. | Specify when reminders are sent and by which supported channels. |
| F-05 | R-07 | Cancellation rules and identity verification are unclear; the requirement also combines multiple obligations. | Unauthorized or confusing cancellations and inconsistent schedule updates. | Split the requirement into atomic requirements and define authentication, cancellation rules, and notifications. |
| F-06 | R-08 | "User-friendly for all age groups" is subjective and has no accessibility criteria. | Elderly patients may be unable to use the system. | Add testable usability/accessibility requirements and an alternative assisted-booking process. |
| F-07 | R-10 | Walk-in booking is covered, but emergency walk-in prioritization is not. | Emergency patients may not be handled appropriately. | Define how receptionists identify and prioritize emergency walk-ins, including the clinic-approved workflow. |
| F-08 | R-11 | The scope of the three-active-appointments limit is unclear. | Online and receptionist bookings may apply different limits. | State that the limit applies across all booking channels, if that is the clinic's intended rule. |
| F-09 | R-12 | "Normal working hours" is not defined. | Availability cannot be verified against a precise schedule. | Specify operating days, hours, time zone, and any planned maintenance exception. |
| F-10 | R-09 | "Stored securely" does not identify access permissions or security controls. | Unauthorized access or disclosure of medical information. | Define role-based access, authentication, audit logging, and applicable data-protection controls. |
| F-11 | R-13 | "As per clinic policy" refers to a policy not included or identified in the SRS. | Payment handling may be implemented inconsistently. | Attach or reference the approved clinic policy and define the system behaviour. |
| F-12 | R-14 | The contents and permitted details of the doctor's daily schedule are not specified. | Doctors may not receive the information needed for their workflow. | Define the schedule fields and access restrictions. |
| F-13 | Stakeholder list | Clinic administrator and data protection officer are listed as users, but their system responsibilities are absent. | Important administration and privacy workflows may be omitted. | Add requirements for each role's permitted tasks and access. |
| F-14 | R-01–R-03; clinic concern | No capacity or performance requirement addresses busy Monday mornings. | Slow responses or booking failures during peak demand. | Define expected concurrent users/booking volume and measurable peak-load performance. |

## Stakeholder Coverage

### 1. Patient
Online booking, reminders, cancellations, accessibility, and appointment limits need clarification.

### 2. Doctor
Appointment duration rules and daily schedule details need clarification.

### 3. Receptionist
Walk-in and emergency walk-in handling need clarification.

### 4. Clinic Administrator
Operating hours, payment policy, and administrative responsibilities need clarification.

### 5. Data Protection Officer
Medical-record access and security controls need clarification.

## Recommendation

Do not approve the SRS in its current form. Ask the software company to resolve the R-04/R-05 contradiction and make the high-risk requirements measurable, testable, and complete.

Re-run the validation checklist against the revised SRS before signing the contract.
