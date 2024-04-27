# iCare, a hospital website management service

## ![developer](https://img.shields.io/badge/Developed%20By%20%3A-Sherida%20Providence-blue) | [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://buymeacoffee.com/asptechinc)

## Screenshots

|                                              **Homepage**                                               |                                               **Admin Dashboard**                                                |                                              **Invoice**                                               |                                               **Doctor List**                                                |
| :-----------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------: |
| <img src="https://github.com/Sherida101/iCare/blob/master/static/screenshots/homepage.png?raw=true"  /> | <img src="https://github.com/Sherida101/iCare/blob/master/static/screenshots/admin_dashboard.png?raw=true"    /> | <img src="https://github.com/Sherida101/iCare/blob/master/static/screenshots/invoice.png?raw=true"  /> | <img src="https://github.com/Sherida101/iCare/blob/master/static/screenshots/admin_doctor.png?raw=true"   /> |

## Functions of the Website

### Admin

- [✔] Sign-up for an account
- [✔] Login with no approval required
- [✔] Register, view, approve, reject and delete a doctor from the hospital
- [✔] Approve doctor(s) who applied for employment in the hospital
- [✔] Admit, view, approve, reject and discharge patients (after a treatment has occurred)
- [✔] Generate and download invoices as pdf documents. Invoices are generated according to medicines' cost, room charge, doctor charge as well as other charges
- [✔] View, book and approve medical appointments that are requested by patients.
- [x]
- [x]
- [x]

### Doctor

- [✔] Apply for employment within the hospital
- [✔] Login with approval required by the hospital administrator. Doctors can only login
- [✔] View patients' details such as medical symptoms, name and mobile number. These patients are assigned to the doctor by the admin
- [✔] View a list of discharged patients once authorised by the admin
- [✔] View all patients' appointments that booked by the admin
- [✔] Delete patients' appointments after a doctor has attended to the appointments
- [x]
- [x]
- [x]

### Patient

- [✔] Create an account in order to be admitted in hospital. Login after approval has been granted by the hospital admin
- [✔] View the details of the doctor whom he or she is assigned to such as the specialisation, mobile number and residential address of the doctor
- [✔] View the status of booked appointments like pending and confirmed. The status is reviewed by the admin.
- [✔] Book appointments which are approved by the admin
- [✔] View and download invoices as a pdf document only when the patient is discharged by the admin

---

## Steps to run project

- Install Python(3.8.10)...ensure that you tick 'add to path' when installing Python
- Open terminal then, execute the following commands :

```
pip install django==3.0.5
pip install django-widget-tweaks
pip install xhtml2pdf
```

- Clone GitHub project
- Navigate to project folder using the terminal then, run the following commands :

```
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py runserver
```

- If you do not have python3 installed, run the commands with py instead of python3 e.g. py manage.py makemigrations

- View the website in the browser by entering the following URL:

```
http://127.0.0.1:8000/
```

## Customise 'Contact Us Page' to make it your own

- In settins.py file, You have to give your email and password

```
EMAIL_HOST_USER = 'youremail@gmail.com'
EMAIL_HOST_PASSWORD = 'your email password'
EMAIL_RECEIVING_USER = 'youremail@gmail.com'
```

- Login to gmail through host email id in your browser and open following link and turn it ON

```
https://myaccount.google.com/lesssecureapps
```

## Drawbacks

- Any user can be an administrator because there is no approval required for an admin account.
- The admin sign-up process can be disabled then,a logic like creating superuser can be used.
- At least one doctor should be in the hospital before a patient can be admitted. Ensure that a doctor is added first.
- Update password first on the Update page of A doctor or patient

# Technologies used 🛠️

- [React](https://reactjs.org/)

## License 📄

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/Sherida101/iCare/blob/master/LICENSE) file for details.

# Reference 👏🏻

- Design ideas were adopted from [sumitkumar1503's Hospital Management project](https://github.com/sumitkumar1503/hospitalmanagement).
