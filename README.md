# Healthcare-Dataset
 This report provides a detailed visual analysis of a healthcare dataset using Power BI and Excel. The dataset contains patient records with details such as demographics, medical conditions, hospital admission details, billing information, and test results.
 The analysis highlights key insights into patient demographics, common medical conditions, financial patterns across insurance providers, hospital resource usage, and clinical outcomes. These insights aim to support data-driven decisions for improving patient care and operational efficiency.

### 1. Demographic Analysis
Age Distribution
•	The majority of patients fall within in  age of 60-90 and 18-40  the age group. 
•	Age group of 0-18 patients is low

 <img width="714" height="345" alt="image" src="https://github.com/user-attachments/assets/4b404d31-5ca2-4ff0-bbc3-fa704807fcdc" />


Gender Breakdown

<img width="668" height="388" alt="image" src="https://github.com/user-attachments/assets/1d16f5c4-40c6-46ca-b11c-051c9dfdff05" />


•	Male: 50%, Female: 49.98% 
•	Gender Brekdown of age group 

<img width="662" height="386" alt="image" src="https://github.com/user-attachments/assets/ba9a22fb-3433-473f-a305-6185713bcf1a" />

          
•	Blood Type Frequency
•	The most common blood types are [O+, A+, A-, B+, B-, AB+, AB-].
•	The rare blood group type is [O-]

<img width="728" height="414" alt="image" src="https://github.com/user-attachments/assets/5241eb11-c8b2-4fa1-91a9-7eeade00ec6d" />

 
### 2. Hospital Admission Trends
Admissions Over Time
•	Admission peaks are observed in eight months potentially linked to seasonal illnesses.

 <img width="673" height="387" alt="image" src="https://github.com/user-attachments/assets/9674f693-c8ff-4357-a01e-1e4cd7becdad" />


Top Hospitals and Doctors
•	Hospital LLC Smith has the highest number of admissions.
•	Each Dr. treated the one patient.
 
<img width="656" height="431" alt="image" src="https://github.com/user-attachments/assets/a51bc71c-0168-472b-a967-355846ae8a61" />


<img width="649" height="383" alt="image" src="https://github.com/user-attachments/assets/62d91637-e06b-4110-b277-2cb782ac2591" />


Admission Types
•	The most frequent type is Elective followed by Emergency.

 
<img width="708" height="405" alt="image" src="https://github.com/user-attachments/assets/27b602b6-7aa8-467a-aa28-1ff95fbedb58" />


### 3. Billing & Insurance
Average Billing Amount by Insurance Provider
•	Highest average billing is associated with Medicare and Blue Cross


 <img width="732" height="414" alt="image" src="https://github.com/user-attachments/assets/216fa321-177b-44de-91f7-cf189114a069" />

  
•	Private rooms correlate with higher billing amounts.


<img width="732" height="359" alt="image" src="https://github.com/user-attachments/assets/961f328d-0290-4377-952e-07d67953e229" />


Insurance Provider Usage
•	Most patients are covered by Cigna and Medicare.


<img width="734" height="353" alt="image" src="https://github.com/user-attachments/assets/088aa345-7676-4be0-8fb0-c3354f09eb37" />



•	
💊 4. Medical Conditions & Treatments
Top Medical Conditions
•	Common diagnoses include Arthritis, Diabetes, Hypertension

 
<img width="726" height="356" alt="image" src="https://github.com/user-attachments/assets/51a834cb-394b-4112-bc65-bf00f8a6ecce" />


Most Prescribed Medications
•	Frequently prescribed medications include Lipitor but more difference to others


<img width="723" height="358" alt="image" src="https://github.com/user-attachments/assets/0a89f23a-998d-4255-9e8d-aa9faf82c98e" />


Length of Stay by Condition
•	Longest average stays are seen in patients with Arthritis


 <img width="731" height="377" alt="image" src="https://github.com/user-attachments/assets/976cbddb-fac9-4760-a514-ffcb946066cd" />


### 5. Test Results & Clinical Insights
Test Results Distribution
•	Most test results 
 
<img width="759" height="371" alt="image" src="https://github.com/user-attachments/assets/60c98c5d-0d1c-4d86-be79-1a925fbe8b83" />


Test Results vs Billing
•	A slight positive correlation was observed between test result levels and billing.

<img width="809" height="384" alt="image" src="https://github.com/user-attachments/assets/550c21e2-1690-4d2c-871e-9050fd119b1b" />



### 6. Discharge & Hospital Stay Patterns
Average Length of Stay
•	Average patient stay: 15.50 days.

 
<img width="740" height="358" alt="image" src="https://github.com/user-attachments/assets/5a956ad4-0a4b-4dca-8131-c8232b63d1ba" />


Discharges by Weekday
•	Highest discharges: Weekday, lowest: weekend

 
<img width="775" height="368" alt="image" src="https://github.com/user-attachments/assets/45e67a3c-d20b-4cec-9dc1-52e712ff5325" />


### Conclusions & Recommendations

•	Patient Demographics: Focus on care planning for middle-aged patients (60-90), who make up the majority.
•	Billing Insight: Room number 391and certain insurance providers lead to higher costs.
•	Gender of male and female equal
•	Hospital Operations: Resource allocation should consider admission peaks.
________________________________________
### Appendix
## Power BI Dashboards
•	Screenshot of dashboard overview

 
<img width="846" height="466" alt="image" src="https://github.com/user-attachments/assets/ddf0d3cf-0fd3-4229-9d86-654687eb96f1" />


 <img width="840" height="471" alt="image" src="https://github.com/user-attachments/assets/86e8e3ef-195b-4d79-99f1-44f2bde27bef" />



DAX Measures Used (Examples)
Created Admission date table by Admission date column


<img width="940" height="371" alt="image" src="https://github.com/user-attachments/assets/fab422a5-aa80-4bc3-bcae-1f13faa3dacc" />

 
Created Discharged date table by Discharged date column
 

<img width="940" height="349" alt="image" src="https://github.com/user-attachments/assets/5c22ba99-cdaf-467c-8466-472ad6f0d1da" />


•	Created Age Group  by using Group function  0-18,18-40,40,60 and 60-90
•	Created Measure for to find how may days patient stay   
•	LengthOfStay = DATEDIFF(healthcare_dataset[Date of Admission], healthcare_dataset[Discharge Date], DAY)
•	Created group for length od stay using group function 1-10,11-20,21-30


### Excel Dashboard Images:


<img width="1684" height="788" alt="1" src="https://github.com/user-attachments/assets/ddcf835a-3186-4786-9e41-3aaf2d357876" />


<img width="1677" height="773" alt="2" src="https://github.com/user-attachments/assets/0c2adc3d-d64e-4018-8b70-87e973ff61cc" />


<img width="1673" height="751" alt="3" src="https://github.com/user-attachments/assets/bd57a0bb-d862-4a07-9eaa-e05687f844d2" />


