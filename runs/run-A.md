
# Validation Checklist Run A

**Reviewer:** Fatima Abid  
**Start time:** [2:00]  
**End time:** [2:30]


| ID | Checklist item | Answer | Evidence / reason |
|---|---|---|---|
| CL-01 | Does the SRS assign a unique identifier to every requirement? | Yes | R-01 to R-14 have unique identifiers. |
| CL-02 | Does each requirement describe one clear system obligation? | No | R-07 combines cancellation, schedule updating, and receptionist notification in one requirement. |
| CL-03 | Does the SRS define a measurable response-time limit for booking requests? | No | R-02 says "quickly" but gives no numerical response-time target or unit. |
| CL-04 | Does the SRS define how simultaneous booking requests are prevented from creating double bookings? | No | R-03 gives no concurrency rule or acceptance criteria showing how simultaneous bookings are prevented. |
| CL-05 | Do the requirements specify one consistent appointment duration rule? | No | R-04 fixes every appointment at 15 minutes, while R-05 lets doctors choose 10–30 minutes. |
| CL-06 | Does the SRS specify how far in advance appointment reminders must be sent? | No | R-06 does not state the reminder lead time. |
| CL-07 | Does the SRS identify the channel used to send appointment reminders? | No | R-06 does not identify a reminder delivery channel. |
| CL-08 | Does the SRS define a cancellation deadline for patients? | No | R-07 says "at any time" but does not define a cancellation cutoff or related rules. |
| CL-09 | Does the SRS specify how a patient's identity is verified before an appointment is cancelled? | No | R-07 does not specify identity verification before cancellation. |
| CL-10 | Does the SRS define measurable usability or accessibility criteria for elderly patients? | No | R-08 uses "user-friendly" but gives no measurable accessibility criteria. |
| CL-11 | Does the SRS specify a process for prioritizing emergency walk-in patients? | No | R-10 supports walk-ins but does not define emergency walk-in prioritization. |
| CL-12 | Does the SRS state whether the three-active-appointments limit applies to online and receptionist bookings? | No | R-11 does not say whether the limit covers both online and receptionist-created bookings. |
| CL-13 | Does the SRS state the exact days and hours when the system must be available? | No | R-12 does not define the exact days or hours meant by "normal working hours." |
| CL-14 | Does the SRS define which user roles may view patient medical records? | No | R-09 does not identify permitted roles for viewing medical records. |
| CL-15 | Does the SRS specify security controls for protecting stored patient records? | No | R-09 says "securely" but does not specify security controls. |
| CL-16 | Does the SRS define the clinic policy for handling overdue payments? | No | R-13 refers to clinic policy without including or identifying that policy. |
| CL-17 | Does the SRS specify the information shown in a doctor's daily schedule? | No | R-14 says doctors can view a daily schedule but does not define the schedule's required contents. |
| CL-18 | Does the SRS define the clinic administrator's system responsibilities? | No | The clinic administrator is listed as a user, but no system responsibilities are specified. |
| CL-19 | Does the SRS define the data protection officer's responsibilities in the system? | No | The data protection officer is listed as a user, but no system responsibilities are specified. |
| CL-20 | Does the SRS specify the booking capacity required for busy Monday mornings? | No | The SRS does not specify capacity or performance expectations for busy Monday mornings. |
