
## Hospital Management System

Hospital Management System (HMS) 🏥 is a comprehensive software solution designed to streamline healthcare operations. 🌟 This system integrates MySQL for robust data management, PHP for server-side scripting, and Bootstrap for responsive web design, ensuring accessibility across devices. 🖥️ HMS facilitates efficient patient management, appointment scheduling, doctor coordination, billing, and administrative tasks, enhancing overall hospital productivity and patient care. With user-friendly interfaces and secure data handling, HMS supports healthcare providers in delivering quality services while maintaining organizational efficiency. 📊

## Table of content <!-- omit from toc -->
- [Steps to run the project in your machine](https://github.com/Shrey2dew/Football-Player-Detection-and-Tracking?tab=readme-ov-file#yolov5)
- [Getting into project](https://github.com/Shrey2dew/Football-Player-Detection-and-Tracking?tab=readme-ov-file#bytetrack)
- [Patient Module](https://github.com/Shrey2dew/Football-Player-Detection-and-Tracking?tab=readme-ov-file#-screenshots)
- [Doctor Module](https://github.com/Shrey2dew/Football-Player-Detection-and-Tracking?tab=readme-ov-file#technologies-used-%EF%B8%8F)
- [Admin Module](https://github.com/Shrey2dew/Football-Player-Detection-and-Tracking?tab=readme-ov-file#project-structure)
- [Updates](https://github.com/Shrey2dew/Football-Player-Detection-and-Tracking/blob/main/README.md#contributors)
- [Technology Stack](https://github.com/Shrey2dew/Football-Player-Detection-and-Tracking?tab=readme-ov-file#license)
- [Contributors](https://github.com/Shrey2dew/Football-Player-Detection-and-Tracking?tab=readme-ov-file#conclusion)


## Steps to run the project in your machine
Download XAMPP control panel [XAMPP](https://www.apachefriends.org/)
### Setup
1. Go to C Drive and open xampp folder.
2. Navigate to htdocs in xampp and **delete** the **index.php** file.
3. Extract the source code zip , downloaded from github and copy paste all it's content in htdocs
4. Copy php path present in xampp folder
        
        C:\xampp\php
    
5. Set up the enviornment variable path

        - search edit the system enviornment variable
        - Go Advanced > environment > user variables > path 
        - Select new and paste the php path

### Starting Apache And MySQL in XAMPP:
![](https://github.com/Shrey2dew/Hospital-Management-System/blob/main/Helping%20Videos/How%20to%20set%20up%20Apache%20and%20Mysql%20in%20Xampp.gif)
###### Follow above video fro setting up Apache and MySQL
1. Select start and admin on MySQL and Apache
2. In Php admin :
        
        - select new on left hand corner
        - give name MyHMSDB and click on create
        - select import > choose file > go to Hospital Management System folder and select myhmsdb.sql file and click import
![](https://github.com/Shrey2dew/Hospital-Management-System/blob/main/Helping%20Videos/Php%20Setup.gif)

### Hooray you have finally setup the HMS system 🎉








## Getting into project
Hospital Management System in php and mysql. This system has a ‘Home’ page from where the patient, doctor & administrator can login into their accounts by toggling the tabs accordingly. Fig 1.1 shows the ‘Home’ page of our project.

The ‘Home’ page consists of 3 modules:
1. Patient Module
2. Doctor Module
3. Admin Module

### Patient Module

This module allows patients to create their account, book an appointment to see a doctor and see their appointment history.

The registration page(in the home page itself) asks patients to enter their First Name, Last Name, Email

Once the patient has created his/her own account after clicking the ‘Register’ button, then he will be redirected to his/her Dashboard

The Dashboard page allows patients to perform two operations:

<div align="left">

 <img src="https://github.com/Shrey2dew/Hospital-Management-System/blob/main/Output/Patient%20Registration.png" width="auto" height="auto" /> 

</div>

**1. Book his/her appointment:**

Here, the patients can able to book their appointments to see a doctor. The appointment form(Fig 1.6) requires patients to select the doctor that they want to see, Date and Time that they want to meet with the doctor. The consultancy fee will be shown accordingly to the patient as it was already determined by the doctor.

After clicking on the ‘Create new entry’ button, the patient will receive an alert that acknowledges the successful appointment of the patient. 

<div align="left">

 <img src="" width="auto" height="auto" /> 

</div>

**2. View patients’ Appointment History:**

Here, the patient can see their appointment history which contains Doctor Name, Consultancy Fee, Appointment Date and Time.(See Fig 1.8).

Once the patient has logged out of his account, if he wants to go into his account again, he can login his account, instead of register his account again. Fig 1.9 shows the login page.
Clicking on ‘Login’ button will redirect the patient to his dashboard page which we have seen earlier

This is how the patient module works. On the whole, this module allows patients to register their account or login their account(if he/she has one), book an appointment and view his/her appointment history.
<div align="left">
 
| Book Appointment | View History | 
| :---         |     :---      |       
| <img src="https://github.com/Shrey2dew/Hospital-Management-System/blob/main/Output/Book%20Apointmnet.png" width="500" height="auto" />  | <img src="https://github.com/Shrey2dew/Hospital-Management-System/blob/main/Output/Appointment%20History.png" width="500" height="auto" />    

</div>

### Doctor Module

The doctors can login into their account which can be done by toggling the tab from ‘Patient’ to ‘Doctor’.Below shows the login form for a doctor. Registration of a doctor account can be done only by admin. We will discuss more about this in Admin Module.

Once the doctor clicking the ‘Login’ button, they will be redirected to their own dashboard which is shown in  

In this page, doctor can able to see their appointments which has been booked by the patients. Fig 1.12 shows the appointment of the doctor ‘Ganesh’ which has been booked by the patient ‘Kenny Sebastian’. This means that the doctor ‘Ganesh’ will have an appointment with the patient ‘Kenny Sebastian’ on 10-10-2019 10AM. 

In real-time, the doctors will have thousands of appointments. It will be easier for a doctor to search for appointment in the case of more appointments. To make it easier, I have a ‘Search’ box in the navigation bar which allows doctors to search for a patient by their contact number.

Once everything is done, the doctor can logout of their account. Thus, in general, a doctor can login into his/her account, view their appointments and search for a patient. This is all about Doctor Module.
<div align="left">
 
| Doctor Username and Password | Appointment List | 
| :---         |     :---      |       
| <img src="https://github.com/Shrey2dew/Hospital-Management-System/blob/main/Output/User%20Name%20and%20Password%20of%20Doctor.png" width="500" height="auto" />  | <img src="https://github.com/Shrey2dew/Hospital-Management-System/blob/main/Output/Doctor%20Appointment%20List.png" width="500" height="auto" />    

</div>

### Admin Module
   
This module is the heart of our project where an admin can see the list of all patients. Doctors and appointments and the feedback/queries received from the ‘Contact’ page. Also admin can add doctor too. 

Login into admin account can be done by toggling into admin tab of the Home page. Fig 1.13 shows the login page for admin.
        
        username: admin
        password: admin123 

On clicking the ‘Login’ button, the admin will be redirected to his/her dashboard.

This module allows admin to perform five major operations:

**1. View the list of all patients registered:**

Admin can able to view all the patients registered. This includes the patients’ First Name, Last Name, Email ID, Contact Number and Password.As like in doctor module, admin can also search for a patient by their contact number in the search box.
  
**2. View the list of all doctors registered:**

Details of the doctors can also be viewed by the admin. This details include the Name of the doctor, Password, Email and Consultancy fees, shown in Fig 1.16. Searching for a doctor can be done by using the doctor’s Email ID in the search box.

**3. View the Appointment lists:**

Admin can also able to see the entire details of the appointment that shows the appointment details of the patients with their respective doctors. This includes the First Name, Last Name, Email and Contact Number of patients, doctor’s name, Appointment Date, Time and the Consultancy Fees. (See Fig 1.17). 
  
**4. Add Doctor:**

Admin alone can add a new doctor since anyone can register as a doctor if we put this section on the home page. This form asks Doctor’s Name, Email ID, Password and his/her Consultancy Fees.(See Fig 1.18)
  
After adding a new doctor, if we check the doctor’s list, we will see the details of new doctor is added to the list as shown in the Fig 1.19
  
**5. View User’s feedback/Queries:**

Admin is allowed to view the feedback/Query that has been given by the user in the ‘Contact’ page (Refer Fig 1.3). This includes User’s Name, Email Id, Contact Number and the message(Feedback/ Query) as shown in the Fig 1.20.
  
Taking everything into consideration, admin can able to view the details of patients and doctors, appointment details, Feedback by the user and can add a new doctor. Once everything is done, the admin can logout from his account.
<div align="left">

 <img src="https://github.com/Shrey2dew/Hospital-Management-System/blob/main/Output/Admin%20Page.png" width="auto" height="auto" /> 

</div>

## Updates

### 1. Cancel Appointments
	
Patients and doctors can able to delete their appointments.
    
If the patient deletes the last record (for doctor Ganesh), then a label "deleted by you" will be displayed in the column 'Current Status' and the action will change to cancel state.
  
Now if we login to the doctor Ganesh's account and view his appointment details, then it will look like this:
  
Similarly doctors can also delete their appointments and patients can view their updated appointment details.
  
### 2. Remove Doctors by Admin

Admin can also delete the doctors from the system. This let admin to have more control over the system.
## Technology Stack ⚙️

1. HTML5/CSS3
2. JavaScript (to create dynamically updating content)
3. Bootstrap (An HTML, CSS, and JS library)
4. XAMPP (A web server by Apache Friends)
5. Php
6. MySQL (An RDBMS that uses SQL)
7. TCPDF (to generate PDFs)
## Contributors 🤝
