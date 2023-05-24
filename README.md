# CV Generator Project
Welcome to my CV generator portfolio project
This is a Django 4.1.4 project.

This project is a simple cv generator website project.

To properly use this project you have to change the path for python in pyvenv.cfg to use the python virtual enviroment.

# About

On this page, the user can fill up the form in the 'form' tab. The data is saved to the database after filling up the form and clicking 'Submit'. 
The 'list' tab displays the names of all users available in the database. Next to the names there is a button 'Download CV' responsible for downloading the pdf CV file. 
Each user has it's own downloading button. Products can only be added through the admin directly in the database

# Technologies

Front-end technologies used in the project:
- HTML

Back-end technologies used in the project:
- Python
- Django

Main functions

- The 'Home' page
- Page with list of all the users
- Downloading pdf files with pdfkit
- Separate html file for generating CV pdf files
- Saving all the user data to the database
- functional navbar
- CV data form

Bootstrap 5 was used to style the website

![CV_1](https://github.com/PiotrWirth/Website_CV_Generator/assets/26605945/1e7f1134-be11-44e6-91aa-ea1899e52726)
![CV_2](https://github.com/PiotrWirth/Website_CV_Generator/assets/26605945/7f985f0b-475f-4834-acd6-1cfc6f772ac3)
![CV_3](https://github.com/PiotrWirth/Website_CV_Generator/assets/26605945/a6f64272-d29f-463b-b63e-ddefb2a365df)


For the generator to work you need to install wkhtmltopdf and change this path in views.py

config = pdfkit.configuration(wkhtmltopdf=r'C:/Users/piotr/OneDrive/Pulpit/Projects/wkhtmltopdf/bin/wkhtmltopdf.exe')
