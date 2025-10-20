# Medical Appointment-No Shows Analysis

### Objective
To clean and preprocess the **Medical Appointment No Shows** dataset, which contains patient appointment information and whether the patient attended their appointment.

### Tools Used
Python and its library Pandas

### Skills Demonstrated
- Using Pandas for cleaning and preprocessing data.
- Handling missing, duplicate, and inconsistent data.
- Standardizing date formats.
- Ensuring data integrity and quality for analysis.

### Steps Performed
- Imported dataset using **Pandas**.
- Checked data types, duplicated data and missing values.
- Converted data types to int, datetime and bool:
  - Standardized `no_show` column to bool ( "YES" → '1' and "NO" → '0')
  - Set numeric columns to proper numeric types.
  - Converted `ScheduledDay` and `AppointmentDay` columns to **datetime**.
- Renamed columns to standardize names.
- Removed rows with unrealistic ages.
- Ensured scheduled date ≤ appointment date.
- Exported dataset to `no_shows_cleaned.csv`.

### 📊 Dataset Overview

| Column | Description |
|---------|--------------|
| `PatientId` | Identification of a patient |
| `AppointmentID` | Identification of each appointment |
| `Gender` | Gender of the patient |
| `ScheduledDay` | Date the appointment was scheduled |
| `AppointmentDay` | The day of the actual appointment |
| `Age` | Patient’s age |
| `Neighbourhood` | Where the appointment takes place |
| `Scholarship` | Whether patient is on scholarship (1/0) |
| `Hipertension` | Hypertension status (1/0) |
| `Diabetes` | Diabetes status (1/0) |
| `Alcoholism` | Alcoholism indicator (1/0) |
| `Handcap` | Disability indicator (1/0) |
| `SMS_received` | 1 or more messages sent to the patient |
| `No-show` | Appointment attendance |
