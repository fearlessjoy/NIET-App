NIET Visitor Sign On/Sign Off Web App

This web application allows visitors to sign on and sign off when visiting the New Zealand Institute of Education and Training (NIET). It includes a user-friendly interface where visitors can input their details, and the app stores their data temporarily to track who is currently on-site. Additionally, the app features a QR code generation for signed-in users and allows visitors to easily sign off before leaving.

Features
Sign On: Visitors can sign on by providing their first name, last name, phone number, and whether they have parked on-site.
Vehicle Registration: If a visitor has parked on-site, they can enter their vehicle registration number.
Sign Off: Visitors can search their name and sign off from the system.
QR Code Generation: Upon successful sign-on, a QR code is generated that corresponds to the visitor's full name.
Back Button: Visitors can navigate back to the main screen from the sign-on or sign-off forms.
Email Notification (Admin): A feature to notify the admin (admin@niet.ac.nz) upon successful sign-on.
Responsive Design: The app is mobile-friendly and adaptable to various screen sizes.
How to Use
Main Screen: Upon loading the app, the visitor sees two buttons: Sign On and Sign Off.

Click Sign On to sign on to the premises.
Click Sign Off to sign off from the premises.
Sign On Process:

Enter your First Name, Last Name, and Phone Number.
Indicate whether you parked on-site. If "Yes," an additional field will appear for your Vehicle Registration Number.
Click Submit. A message will confirm a successful sign-on, and a QR code with your name will be generated.
The admin will be notified via email of your sign-on.
Use the Back button if you wish to return to the main screen without signing on.
Sign Off Process:

Start typing your name in the text box.
A dropdown list will show matching names.
Select your name and click Sign Off. A message will confirm successful sign-off.
Use the Back button if you wish to return to the main screen without signing off.
QR Code: After signing on, a QR code will appear on the screen, containing the visitor's full name.

Project Structure
The app consists of a single index.html file that includes all the necessary HTML, CSS, and JavaScript. The JavaScript handles form submissions, manages visitor data, and generates the QR codes.

HTML Structure
Main Screen: Displays two buttons (Sign On and Sign Off).
Sign On Form: Captures visitor details and optionally vehicle registration number.
Sign Off Form: Allows visitors to select their name from a dropdown list and sign off.
Message Section: Displays feedback for the visitor (e.g., sign-on confirmation, QR code).
CSS Styling
Responsive Design: The app is styled to fit mobile, tablet, and desktop screen sizes.
Buttons: Styled with background colors to distinguish between actions (Sign On, Sign Off, Back).
Forms: Styled with easy-to-read input fields and clear labels.
JavaScript Logic
Form Display: Toggles between the main screen and the sign-on/sign-off forms.
Sign On Logic: Collects visitor information and stores it temporarily, sends sign-in data to the server, and generates a QR code.
Sign Off Logic: Filters visitors based on name input and allows users to sign off.
Back Button: Allows navigation from the forms back to the main screen.
QR Code Generation: Uses the qrcode.js library to generate a QR code upon successful sign-on.
API Endpoints
POST /signin: Sends the visitor's sign-in data to the server.
QR Code
The app uses the qrcode.js library to generate QR codes for visitors upon sign-on. The QR code contains the visitor's full name for identification.

Email Notification (Admin)
Once a visitor successfully signs on, the admin (admin@niet.ac.nz) will receive an email notification with the visitor's information.

Installation
Clone the repository to your local machine.

bash
Copy code
git clone https://github.com/your-username/niet-visitor-app.git
Install necessary dependencies for running the app, if required (e.g., setting up a server to handle email notifications).

Open the index.html file in your preferred browser.

Dependencies
qrcode.js: A JavaScript library used for generating QR codes.
Future Improvements
Integration with a database to persist visitor data.
Implementing authentication for the admin.
Enhanced styling and UI for better user experience.
License
This project is licensed under the MIT License.
