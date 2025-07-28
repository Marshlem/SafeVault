SafeVault /n
SafeVault is a secure web application designed to manage sensitive data, including user credentials and financial records. The goal of this project is to provide a secure, easy-to-use platform that ensures user data is protected from common vulnerabilities such as SQL injection and Cross-Site Scripting (XSS). SafeVault implements best practices for secure coding, user authentication, authorization (role-based access control), and input validation.
Features
•	Input Validation: Ensures that all user inputs are sanitized and validated to prevent common attacks like SQL injection and XSS.
•	Authentication: Verifies user credentials during login, securely handling password storage with bcrypt hashing.
•	Role-Based Access Control (RBAC): Restricts access to certain features based on user roles, such as Admin and User.
•	Secure Database Queries: Uses parameterized queries to interact with the database, preventing SQL injection vulnerabilities.
•	Cross-Site Scripting (XSS) Prevention: Sanitizes and escapes user-generated content to prevent script injections.
Installation
1.	Clone the repository:
git clone https://github.com/Marshlem/SafeVault.git
2.	Navigate to the project directory:
cd SafeVault
3.	Install dependencies:
o	Ensure you have the necessary .NET runtime installed.
o	Run the following command to restore the required packages:
dotnet restore
4.	Build and run the project:
dotnet build
dotnet run
5.	Open your browser and navigate to http://localhost:5000 to access the application.
Security Features
•	SQL Injection Prevention: All database queries use parameterized statements to safely handle user input, preventing malicious queries.
•	XSS Protection: User input is sanitized using HTML encoding, ensuring that any user-generated content (such as usernames or comments) is safe from script injection attacks.
•	Password Hashing: User passwords are hashed using bcrypt before being stored in the database, ensuring passwords are not stored in plaintext.
Tests
•	SQL Injection Tests: Test cases are included to verify that SQL injection attempts are blocked.
•	XSS Tests: The system is tested for Cross-Site Scripting vulnerabilities, ensuring that malicious scripts are not executed.
•	Authentication Tests: Valid and invalid user login scenarios are tested to ensure proper authentication.
To run the tests:
dotnet test
Contributing
1.	Fork this repository.
2.	Create a new branch (git checkout -b feature-name).
3.	Commit your changes (git commit -m 'Add new feature').
4.	Push to the branch (git push origin feature-name).
5.	Create a pull request.
License
This project is licensed under the MIT License - see the LICENSE file for details.

