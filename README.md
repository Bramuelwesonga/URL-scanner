# URL-scanner
URL Scanner is a Flask-based web application that allows users to scan URLs for potential security threats using the VirusTotal API. It provides a user-friendly interface for uploading files and scanning URLs, with integration for user registration, login, and email notifications.

**Features**
User Registration and Login: Users can create accounts securely and log in to access the URL scanning features.

File Upload and Scanning: Allows users to upload files, which are scanned for threats using the VirusTotal API.

URL Scanning: Provides the capability to scan URLs directly for security risks using the VirusTotal API.

Email Notifications: Sends email notifications upon form submission for user interaction or contact.
**Technologies Used**
Flask: Python web framework used for backend development.

SQLAlchemy: Python SQL toolkit and Object-Relational Mapping (ORM) library for database management.

Flask-WTF: Flask extension for handling web forms and validations.

Flask-Bcrypt: Flask extension for hashing passwords.

Flask-Bootstrap: Flask extension for integrating Bootstrap CSS framework.

Flask-Mail: Flask extension for sending email messages.

VirusTotal API: External API used for scanning files and URLs for security threats.
Clone the Repository:
**Installation and Setup**
bash
Copy code
git clone https://github.com/your-username/url-scanner.git
cd url-scanner
Install Dependencies:

Copy code
pip install -r requirements.txt
Set Environment Variables:

Create a .env file in the root directory:
makefile
Copy code
SQLALCHEMY_DATABASE_URI='sqlite:///app.db'
SECRET_KEY='your_secret_key'
UPLOAD_FOLDER='static/files'
MAIL_SERVER='smtp.gmail.com'
MAIL_PORT=465
MAIL_USERNAME='your_email@gmail.com'
MAIL_PASSWORD='your_email_password'
MAIL_USE_TLS=False
MAIL_USE_SSL=True
VIRUS_TOTAL_API_KEY='your_virustotal_api_key'
Replace placeholders with your actual configuration details.
Initialize the Database:

csharp
Copy code
flask db init
flask db migrate -m "Initial migration"
flask db upgrade
Run the Application:

arduino
Copy code
flask run
Access the Application:
Open a web browser and go to http://localhost:5000 to access the URL Scanner application.

Usage
Register/Login: Create a new user account or log in with existing credentials.

Dashboard: Upload files to scan for security threats using the VirusTotal API.

Scan URL: Enter a URL to scan it for potential security risks.

Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

