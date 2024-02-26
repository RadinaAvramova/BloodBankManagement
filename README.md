# Blood Bank Management System
Welcome to the Blood Bank Management System! This system is designed to streamline the process of managing blood donation, storage, and distribution in blood banks and blood donation centers. It provides a centralized platform for blood bank administrators to efficiently manage donor information, blood inventory, donation requests, and more.

## Features
1. **Donor Management:** Maintain a database of blood donors, including their personal information, medical history, blood type, and donation records.

2. **Blood Inventory:** Track the inventory of blood units available in the blood bank, including details such as blood type, quantity, expiration date, and storage location.

3. **Donation Requests:** Receive and process donation requests from hospitals, clinics, and other medical facilities, ensuring timely delivery of blood units to meet patient needs.

4. **Blood Testing and Screening:** Perform blood testing and screening procedures to ensure the safety and quality of donated blood before it is accepted into the inventory.

5. **Blood Transfusion Management:** Manage blood transfusions by recording recipient information, matching compatible blood units from the inventory, and tracking transfusion history.

6. **Donor Recruitment and Outreach:** Implement donor recruitment and outreach initiatives to encourage blood donation and increase donor participation in community blood drives.

7. **Reports and Analytics:** Generate reports and analytics on donor demographics, donation trends, blood inventory levels, and other key metrics to inform decision-making and improve operations.

### Admin
- Create Admin account using following command
```
py manage.py createsuperuser
```
- After Login, can see Unit of blood of each blood group available, Number Of Donor, Number of blood request, Number of approved request, Total Unit of blood on Dashboard.
- Can View, Update, Delete Donor.
- Can View, Update, Delete Patient.
- Can View Donation Request made by donor and can approve or reject that request based on disease of donor.
- If Donation Request approved by admin then that unit of blood added to blood stock of that blood group.
- If Donation Request rejected by admin then 0 unit of blood added to stock.
- Can View Blood Request made by donor / patient and can approve or reject that request.
- If Blood Request approved by admin then that unit of blood reduced from blood stock of that blood group.
- If Blood Request rejected by admin then 0 unit of blood reduced from stock.
- Can see history of blood request.
- Can Update Unit Of Particular Blood Group.


### Donor
- Donor can create account by providing basic details.
- After Login, Donor can donate blood, After approval from admin only, blood will be added to blood stock.
- Donor can see their donation history with status (Pending, Approved, Rejected).
- Donor can also request for blood from blood stock.
- Donor can see their blood request history with status.
- Donor can see number of blood request Made, Approved, Pending, Rejected by Admin on their dashboard.
> **_NOTE:_**  Donor can donate blood and can also request for blood.





### Patient
- Create account (No Approval Required By Admin, Can Login After Signup)
- After Login, Can see number of blood request Made, Approved, Pending, Rejected by Admin on their dashboard.
- Patient can request for blood of specific blood group and unit from blood stock.
- Patient can see their blood request history with status (Pending, Approved, Rejected).

---

## HOW TO RUN THIS PROJECT
- Install Python(3.7.6) (Dont Forget to Tick Add to Path while installing Python)
- Download This Project Zip Folder and Extract it
- Move to project folder in Terminal. Then run following Commands :

```
python -m pip install -r requirements. txt
```

```
py manage.py makemigrations
py manage.py migrate
py manage.py runserver
```
- Now enter following URL in Your Browser Installed On Your Pc
```
http://127.0.0.1:8000/
```

## Usage
1. **Login:** Log in to the application using your administrator credentials to access the dashboard and administrative functionalities.

2. **Manage Donors:** Add new donors, update existing donor information, view donation history, and search for donors based on criteria such as blood type or location.

3. **Manage Blood Inventory:** Add new blood units to the inventory, update inventory levels, track expiration dates, and allocate blood units for donation requests or transfusions.

4. **Process Donation Requests:** Receive donation requests from medical facilities, verify eligibility, allocate appropriate blood units from the inventory, and arrange for delivery or pickup.

5. **Generate Reports:** Generate reports on donor demographics, donation statistics, blood inventory levels, and other metrics to monitor performance and compliance with regulatory requirements.

## Customization
Customize the Blood Bank Management System to suit the specific needs of your organization by adding or modifying features, integrating with external systems (e.g., hospital information systems), and adapting workflows to align with organizational policies and procedures.
