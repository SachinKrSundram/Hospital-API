# Information about API:
### Theme:
- We’re going to design an API for the doctors of a Hospital which has been allocated by the
govt for testing and quarantine + well being of COVID-19 patients
- There can be 2 types of Users
- Doctors
- Patients
- Doctors can log in
- Each time a patient visits, the doctor will follow 2 steps
- Register the patient in the app (using phone number, if the patient already exists, just
return the patient info in the API)
- After the checkup, create a Report
- Patient Report will have the following fields
- Created by doctor
- Status (You can use enums if you want to):
- Can be either of: [Negative, Travelled-Quarantine, Symptoms-Quarantine,
Positive-Admit]

- Date

# Instructions about SetUp:

First start with downloading the code and and write npm install on code editor, it will install all dependencies on your editor.
You will need a code editor and mongoDB setup on your computer.
We will use postman to check the api is working or not,So download postman on your computer.

1.Now use this **http://localhost:5000/api/v1/doctors/register** route to register doctor in API and add the info as shown in image

![Screenshot (176)](https://user-images.githubusercontent.com/99536825/233152421-f7d0857f-311f-4d57-a19b-46bafc4bf02a.png)


2.Use this **http://localhost:5000/api/v1/doctors/login** to login as a doctor and add info as shown in image

![Screenshot (170)](https://user-images.githubusercontent.com/99536825/233152486-0bfb8dcd-d889-4004-a43e-498f3e271a93.png)


3.Use this **http://localhost:5000/api/v1/patients/register** and add the token in authorization area which is recieved in second point

![Screenshot (171)](https://user-images.githubusercontent.com/99536825/233152570-37706531-6060-4ad8-8c9c-feb593eb7552.png)


4. Use this **http://localhost:5000/api/v1/patients/62c31cc86a84003324d04cb5/create_report** to create report and add status you can see the types of 
   status in report model.

![Screenshot (174)](https://user-images.githubusercontent.com/99536825/233152807-55e99777-cad0-4cb7-a6e5-082ed98a8994.png)


5. Use this **http://localhost:5000/api/v1/patients/62c31cc86a84003324d04cb5/all_reports** to get all the reports.

![Screenshot (177)](https://user-images.githubusercontent.com/99536825/233153796-ebf07eb6-4c07-4169-98b7-f09f6fbcf491.png)


### Author
(@SachinKrSundram)[https://github.com/SachinKrSundram]




