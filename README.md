# Hospital-Managment-system

Hospital Management System using MySQL, Php and Bootstrap

Video Demo : Hospital Management System - Youtube

Live Demo : Hospital Management System - 000webhost by Kishan

Need to work on:
Ability to accept the appointment by the doctor to acknowledge the patient that their appointment has been approved.
User should not be allowed to register if he/she tries to provide the already registered email ID.
The password should be encrypted and the password field shouldn't be displayed in the admin panel.
Implementation of pagination for all the list view across the application.
Bug fix - Bill payment receipt contains multiple record if the patient has associated with the same doctor multiple times.
Addition of more fields in the prescription statement to make it more specific one.
Addition of more details on payment - such as date of the payment made, amount paid, etc.
Implementation of export button in admin module to export all details to an excel sheet.
Prerequisites
Install XAMPP web server
Any Editor (Preferably VS Code or Sublime Text)
Any web browser with latest version
Languages and Technologies used
HTML5/CSS3
JavaScript (to create dynamically updating content)
Bootstrap (An HTML, CSS, and JS library)
XAMPP (A web server by Apache Friends)
Php
MySQL (An RDBMS that uses SQL)
TCPDF (to generate PDFs)
Steps to run the project in your machine
Download and install XAMPP in your machine
Clone or download the repository
Extract all the files and move it to the 'htdocs' folder of your XAMPP directory.
Start the Apache and Mysql in your XAMPP control panel.
Open your web browser and type 'localhost/phpmyadmin'
In phpmyadmin page, create a new database from the left panel and name it as 'myhmsdb'
Import the file 'myhmsdb.sql' inside your newly created database and click ok.
Open a new tab and type 'localhost/foldername' in the url of your browser
Hurray! That's it!
SOFTWARES USED
XAMPP was installed on the Ubuntu 19.04 machine and APACHE2 Server and MySQL were initialized. And, files were built inside opt/lampp/htdocs/myhmsp
Sublime Text 3.2 was used as a text editor.
Google Chrome Version 77.0.3865.90 was used to run the project (localhost/myhmsp was used as the url).
Starting Apache And MySQL in XAMPP:
The XAMPP Control Panel allows you to manually start and stop Apache and MySQL. To start Apache or MySQL manually, click the ‘Start’ button under ‘Actions’.



GETTING INTO THE PROJECT:
Hospital Management System in php and mysql. This system has a ‘Home’ page from where the patient, doctor & administrator can login into their accounts by toggling the tabs accordingly. Fig 1.1 shows the ‘Home’ page of our project.

image

'About Us' page (Fig 1.2) allows us to get some more information about the quality and the services of the hospital.

image

‘Contact’ page allows users to provide feedback or queries about the services of the hospital. Fig 1.3 shows the ‘Contact’ page.

image

The ‘Home’ page consists of 3 modules:

Patient Module
Doctor Module
Admin Module
Patient Module:
      This module allows patients to create their account, book an appointment to see a doctor and see their appointment history. The registration page(in the home page itself) asks patients to enter their First Name, Last Name, Email ID, Contact Number, Password and radio buttons to select their gender.

image

Once the patient has created his/her own account after clicking the ‘Register’ button, then he will be redirected to his/her Dashboard(Fig 1.5).

image

The Dashboard page allows patients to perform two operations:

1. Book his/her appointment:

      Here, the patients can able to book their appointments to see a doctor. The appointment form(Fig 1.6) requires patients to select the doctor that they want to see, Date and Time that they want to meet with the doctor. The consultancy fee will be shown accordingly to the patient as it was already determined by the doctor.

image

After clicking on the ‘Create new entry’ button, the patient will receive an alert that acknowledges the successful appointment of the patient.(See Fig 1.7)

image

2. View patients’ Appointment History:

      Here, the patient can see their appointment history which contains Doctor Name, Consultancy Fee, Appointment Date and Time.(See Fig 1.8).

image

Once the patient has logged out of his account, if he wants to go into his account again, he can login his account, instead of register his account again. Fig 1.9 shows the login page. Clicking on ‘Login’ button will redirect the patient to his dashboard page which we have seen earlier (Fig 1.5)

image

This is how the patient module works. On the whole, this module allows patients to register their account or login their account(if he/she has one), book an appointment and view his/her appointment history.

Doctor Module:
      The doctors can login into their account which can be done by toggling the tab from ‘Patient’ to ‘Doctor’. Fig 1.10 shows the login form for a doctor. Registration of a doctor account can be done only by admin. We will discuss more about this in Admin Module.

image

Once the doctor clicking the ‘Login’ button, they will be redirected to their own dashboard which is shown in Fig 1.11

image

In this page, doctor can able to see their appointments which has been booked by the patients. Fig 1.12 shows the appointment of the doctor ‘Ganesh’ which has been booked by the patient ‘Kenny Sebastian’ (Fig 1.6). This means that the doctor ‘Ganesh’ will have an appointment with the patient ‘Kenny Sebastian’ on 10-10-2019 10AM.

image

In real-time, the doctors will have thousands of appointments. It will be easier for a doctor to search for appointment in the case of more appointments. To make it easier, I have a ‘Search’ box in the navigation bar (See Fig 1.12) which allows doctors to search for a patient by their contact number.       Once everything is done, the doctor can logout of their account. Thus, in general, a doctor can login into his/her account, view their appointments and search for a patient. This is all about Doctor Module.

Admin Module:
      This module is the heart of our project where an admin can see the list of all patients. Doctors and appointments and the feedback/queries received from the ‘Contact’ page. Also admin can add doctor too.       Login into admin account can be done by toggling into admin tab of the Home page. Fig 1.13 shows the login page for admin.       username: admin, password: admin123

image

On clicking the ‘Login’ button, the admin will be redirected to his/her dashboard as shown in Fig 1.14.

image

This module allows admin to perform five major operations:

1. View the list of all patients registered:

      Admin can able to view all the patients registered. This includes the patients’ First Name, Last Name, Email ID, Contact Number and Password. (See Fig 1.15).As like in doctor module, admin can also search for a patient by their contact number in the search box.

image

2. View the list of all doctors registered:

      Details of the doctors can also be viewed by the admin. This details include the Name of the doctor, Password, Email and Consultancy fees, shown in Fig 1.16. Searching for a doctor can be done by using the doctor’s Email ID in the search box.

image

3. View the Appointment lists:

      Admin can also able to see the entire details of the appointment that shows the appointment details of the patients with their respective doctors. This includes the First Name, Last Name, Email and Contact Number of patients, doctor’s name, Appointment Date, Time and the Consultancy Fees. (See Fig 1.17).

image

4. Add Doctor:

      Admin alone can add a new doctor since anyone can register as a doctor if we put this section on the home page. This form asks Doctor’s Name, Email ID, Password and his/her Consultancy Fees.(See Fig 1.18)

image

After adding a new doctor, if we check the doctor’s list, we will see the details of new doctor is added to the list as shown in the Fig 1.19

image

5. View User’s feedback/Queries:

      Admin is allowed to view the feedback/Query that has been given by the user in the ‘Contact’ page (Refer Fig 1.3). This includes User’s Name, Email Id, Contact Number and the message(Feedback/ Query) as shown in the Fig 1.20.

image

      Taking everything into consideration, admin can able to view the details of patients and doctors, appointment details, Feedback by the user and can add a new doctor. Once everything is done, the admin can logout from his account.

Updates
1. Cancel Appointments
      Patients and doctors can able to delete their appointments.

image

If the patient deletes the last record (for doctor Ganesh), then a label "deleted by you" will be displayed in the column 'Current Status' and the action will change to cancel state.

image

Now if we login to the doctor Ganesh's account and view his appointment details, then it will look like this:

image

Similarly doctors can also delete their appointments and patients can view their updated appointment details.

2. Remove Doctors by Admin
      Admin can also delete the doctors from the system. This let admin to have more control over the system.

image

Star History
Star History Chart

About
Hospital Management System using php and mysql

Topics
mysql bootstrap php xampp hospital-management fullstack-development hospital-appointment-booking hospital-management-system
Resources
 Readme
 Activity
Stars
 589 stars
Watchers
 25 watching
Forks
 154 forks
Report repository
Releases
No releases published
Packages
No packages published
Languages
PHP
91.4%
 
CSS
3.7%
 
SCSS
2.8%
 
JavaScript
1.9%
 
Hack
0.1%
 
