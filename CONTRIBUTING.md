# Contributing Guide



Thank you for your interest in contributing to the **Property Management System** project! This project is built using **ASP.NET API**. We welcome any improvements, bug fixes, and new features.

## How to Contribute



### 1. Environment Setup



To work with the project, you will need:

* **.NET 8.0 SDK** (or the current version used in the project)


* IDE of your choice: **Visual Studio 2022**, **JetBrains Rider**, or **VS Code**

* DBMS specified in the `appsettings.json` configuration (e.g., PostgreSQL / MS SQL Server)



### 2. Steps to Submit Changes



1. Make a **Fork** of the repository.


2. Clone your fork to your local machine:


```bash
git clone https://github.com/your-profile/Diplom_project_2024.git

```



```
3. Create a new branch for your task with a clear prefix:[cite: 1]
   * `feature/feature-name` — for new features (e.g., `feature/booking-chat`)[cite: 1]
   * `bugfix/bug-description` — for bug fixes (e.g., `bugfix/auth-validation`)[cite: 1]
4. Make your changes and ensure the project compiles successfully:[cite: 1]
   ```bash
   dotnet build

```

5. Run tests (if available):


```bash

```



dotnet test

```
6. Commit the changes and push them to your fork:[cite: 1]
   ```bash
git push origin feature/feature-name

```

7. Open a **Pull Request (PR)** to the `main` or `develop` branch of the main repository.



## Code Style Requirements



Since the project is built on **ASP.NET API**, we adhere to standard Microsoft C# conventions:

* **Architecture**: Maintain separation of concerns. API logic (controllers, DTOs, middleware) should be separated from business logic and data access.


* **RESTful API**: New endpoints must comply with REST standards (proper use of HTTP methods `GET`, `POST`, `PUT`, `DELETE`, and response status codes).


* **Validation**: All incoming data models must pass validation (using DataAnnotations or FluentValidation), especially in the registration, booking, and role management sections.


* **Security**: When adding new endpoints, do not forget to configure authorization attributes (`[Authorize]`) according to user roles (Administrator, Landlord, Client).



## Reporting Bugs and Suggestions



If you find a bug or want to suggest an improvement (for example, the built-in messaging system described in the README):

* Create a new **Issue** in the repository.


* Provide a detailed description of the suggestion or steps to reproduce the bug.



---

Thank you for your contribution to the project's development!
