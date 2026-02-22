# 📖 Bookmate

Bookmate is a fullstack web application for managing books and quotes, built with an Angular frontend and a C# (ASP.NET Core) backend.

The application allows users to register, log in, and manage books and quotes through a secure REST API.  
A strong focus of this project has been authentication and authorization, demonstrating secure user handling and protected API routes.

---

## 🚀 Live Demo

🔗 **Live Application:** earnest-vacherin-96975e.netlify.app
🔗 **API Endpoint:** https://bookapp-qs07.onrender.com/api

---

## ✨ Key Features

- User Registration & Login
- JWT Authentication & Authorization
- My Books / My Quotes
- Add / Update / Delete Books & Quotes
- Light / Dark Mode Toggle
- Responsive Design
- REST API Integration between Angular and ASP.NET Core

---

## 🔐 Authentication & Authorization

Bookmate implements JWT-based authentication using ASP.NET Core.

### Authentication Flow

1. User registers via `/api/auth/register`
2. User logs in via `/api/auth/login`
3. On successful login, a JWT token is generated
4. The token includes user claims and expiration time
5. Protected endpoints require a valid JWT in the Authorization header

### Security Features

- Input validation and trimming
- Case-insensitive username handling
- Minimum username and password length validation
- Duplicate username prevention
- Token-based authentication using HMAC SHA256 signing
- Configurable JWT key, issuer, and audience via `appsettings.json`
- Token expiration (1 hour)

This demonstrates secure client–server authentication and protected API route handling.

Note: Passwords are stored in-memory for demonstration purposes only.

---

## 🖥 Tech Stack

| Frontend | Backend | Data Handling |
|----------|----------|---------------|
| Angular | ASP.NET Core Web API | In-memory data storage |
| TypeScript | C# | Temporary collection (resets on restart) |
| HTML | | |
| SCSS | | |

---

## 📸 Screenshots

### Login Page
![Login](./screenshots/login.png)

### Book List (Desktop)
![Book List Desktop](./screenshots/book-list-desktop.png)

### Book List (Mobile)
![Book List Mobile](./screenshots/book-list-mobile.png)

### Add Book Form
![Add Book](./screenshots/add-book.png)

### Light / Dark Mode
![Theme Toggle](./screenshots/theme-toggle.gif)

---

## 🛠 Installation

### Backend (ASP.NET Core)

```bash
cd BookApi
dotnet restore
dotnet run
```
API runs on: http://localhost:8080

---

### Frontend (Angular)

```bash
cd book-app
npm install
ng serve
```
Frontend runs on: http://localhost:4200

## 👩‍💻 Author

[Michelle Lee](https://github.com/ritsumel)