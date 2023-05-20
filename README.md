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

![1doctors_register](https://github.com/Yashas682/Hospital_api/assets/91604926/8d497fb3-120e-4d4d-97ac-f08c9b76c78d)

2.Use this **http://localhost:5000/api/v1/doctors/login** to login as a doctor and add info as shown in image

![2doctors_login](https://github.com/Yashas682/Hospital_api/assets/91604926/764346f0-1794-4906-81d2-876ef3fd1e0b)

3.Use this **http://localhost:5000/api/v1/patients/register** and add the token in authorization area which is recieved in second point

![3 pat_reg (2)](https://github.com/Yashas682/Hospital_api/assets/91604926/58b15784-936b-4f5d-a541-c8f22cca97e1)
![3 1pat_reg (2)](https://github.com/Yashas682/Hospital_api/assets/91604926/10e3214c-f103-4235-bf96-134424cd3351)

4. Use this **http://localhost:5000/api/v1/patients/62c31cc86a84003324d04cb5/create_report** to create report and add status you can see the types of 
   status in report model.

![image](https://user-images.githubusercontent.com/74106414/236742216-a4684b3b-7e2f-4c2e-a24a-0cf0818d7701.png)


5. Use this **http://localhost:5000/api/v1/patients/62c31cc86a84003324d04cb5/all_reports** to get all the reports.

![image](https://user-images.githubusercontent.com/74106414/236742229-ad057a9b-3b03-4496-bf55-36f1bced526f.png)
