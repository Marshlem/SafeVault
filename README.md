# 🛡️ SafeVault

**SafeVault** is a secure web application designed to manage sensitive user data, including credentials and financial records. With a focus on security, SafeVault implements robust authentication, input sanitization, and security best practices to protect against common vulnerabilities such as SQL injection and XSS. Built with **ASP.NET Core**, **EF Core**, and modern security techniques, SafeVault provides a scalable solution for managing sensitive data securely.

## 🧠 Features

- **Role-Based Access Control (RBAC)**: Restrict access to sensitive features based on user roles.
- **JWT Authentication**: Secure user authentication with JWT tokens stored in **HttpOnly cookies**.
- **Input Validation**: Prevent XSS and SQL Injection by sanitizing user inputs and using parameterized queries.
- **Password Hashing**: Store passwords securely using **bcrypt** hashing.
- **Test Coverage**: Comprehensive tests including **security tests**, **unit tests**, and **integration tests**.

## 🔐 Security Highlights

- **Input Validation**: Ensures that all user inputs are validated and sanitized, preventing SQL injection and XSS attacks.
- **Secure Token Generation**: Utilizes **cryptographically secure techniques** for token generation and validation.
- **OWASP Best Practices**: Follows OWASP guidelines to mitigate common vulnerabilities.
- **Role Authorization**: Restrict access to sensitive data and features based on user roles and claims.

## 🧪 Testing Strategy

Each component—Core, Data, Web—is backed by a dedicated test project:

- **Unit Tests**: For business logic and user authentication.
- **Integration Tests**: For EF Core operations and data access.
- **Security Tests**: Simulating SQL injection, XSS, and RBAC bypass attempts.

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/Marshlem/SafeVault.git
```
### 2. Apply EF Core Migrations
```bash
dotnet ef database update --project SafeVault.Data
```
### 3. Run the Web Project
```bash
dotnet run --project SafeVault.Web
```

## 🛠️ Technologies
ASP.NET Core

Razor Pages

Entity Framework Core

ASP.NET Core Identity

bcrypt

xUnit

## 📝 License
This project is licensed under the MIT License. See the LICENSE file for more details.

## 🤝 Acknowledgments
Special thanks to Microsoft Copilot for assisting with secure code generation, vulnerability detection, and test automation, which contributed significantly to the development of SafeVault.
