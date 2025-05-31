# MSCSUP-AMS
Final_Project

Our Municipal of Sta. Cruz Sports Committee Program and Activity
Monitoring System with Online Registration
implements several security measures to protect against common web vulnerabilities and ensure data integrity:

- **Cross-Site Request Forgery (CSRF) Protection**: All forms and state-changing requests include CSRF tokens validated on the server side to prevent unauthorized requests.
- **Session Management**: Secure, HTTP-only cookies are used for sessions, with session regeneration to prevent fixation attacks.
- **Input Validation and Sanitization**: User inputs are validated and sanitized to prevent SQL Injection, XSS, and other injection attacks.
- **Password Security**: Passwords are hashed using PHP's `password_hash()` function with the bcrypt algorithm.
- **Access Control**: Role-based access control restricts user permissions and prevents unauthorized data access.
- **Error Handling**: Detailed errors are logged server-side, while user-facing messages are generic to avoid information disclosure.
- **Secure File Uploads and QR Code Handling**: Uploaded files and QR code data are validated and sanitized to prevent injection and malware risks.

### Reporting Vulnerabilities

If you discover a security vulnerability, please report it responsibly by contacting the project maintainer directly rather than posting it publicly. Your responsible disclosure helps protect users.

---

You can customize this section based on your specific security features.

---

If you want, I can help you draft a full README template for your entire project including:

- Project description
- Installation instructions
- Usage
- Features
- Security notices (with your specific security code explanation)
- Contribution guidelines
- License info

Would you like me to do that? Or just the security part for now?

## Features

- User authentication with secure login and signup
- Role-based access control to restrict user permissions
- CSRF protection implemented on all forms to prevent unauthorized requests
- Robust session management with HTTP-only cookies and session regeneration
- Anti-bruteforce attack protection by limiting failed login attempts and implementing lockout timers
- Admin and user dashboards for comprehensive system management
- Detailed error handling and logging for security and troubleshooting
- Integration of SweetAlert2 for user-friendly alert messages

- google drive link (https://drive.google.com/drive/folders/1bh7N87Zipe1QafnVWIqMqerR6ET2OLrJ?usp=drive_link)

How to Run the System on Another Computer
To set up and run the Municipal of Sta. Cruz Sports Committee Program and Activity Monitoring System with Online Registration on a different computer, follow these steps:

📁 1. Clone or Download the Repository
Open your terminal or Git Bash.

Run:
git clone https://github.com/EDMardoquio/MSCSUP-AMS
Or download the ZIP file and extract it.

🧱 2. Set Up Your Environment
Make sure the target machine has the following installed:

XAMPP (includes Apache & MySQL)

A web browser (Chrome, Firefox, etc.)

Optional: VS Code for code editing

🛠️ 3. Import the Database
Start Apache and MySQL via XAMPP.

Go to http://localhost/phpmyadmin.

Create a new database (e.g., sports_monitoring).

Import the SQL file:

Click the Import tab.

Choose the .sql file located in the /docs or /database folder of the project.

Click Go.

📂 4. Place the Project in htdocs
Copy the entire project folder to:

makefile
Copy
Edit
C:\xampp\htdocs\
🌐 5. Configure Database Connection
Open /src/includes/db_config.php (or wherever your DB config is located).

Set the database credentials:

Edit
$host = 'localhost';
$user = 'root';
$pass = '';
$dbname = 'sports_monitoring';
🚀 6. Run the System
Open a browser and go to:

arduino
Copy
Edit
http://localhost/your-project-folder/
🔐 7. Default Login (If applicable)
Admin: admin-123
User:  admin

⚠️ Don’t forget to change default credentials and configure permissions for production.
