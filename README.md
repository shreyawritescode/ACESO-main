# ACESO — User Authentication Web App

**ACESO** is a full-stack web application with **user authentication** built using Node.js, Express, MongoDB, and EJS. It allows users to register and log in securely with MD5-hashed passwords and session management.

## Features

- User **registration** with email and password
- Secure **login** with MD5 password hashing
- MongoDB user data persistence
- Dynamic EJS-rendered pages (home, login, register, secrets)
- Environment-based configuration via `.env` (dotenv)
- Static assets served from `public/` directory

## Tech Stack

| Technology | Purpose |
|---|---|
| Node.js | Server-side runtime |
| Express.js | Web framework |
| MongoDB + Mongoose | Database and ODM |
| EJS | Templating engine |
| MD5 | Password hashing |
| dotenv | Environment variable management |
| body-parser | Request parsing middleware |

## Project Structure

```
ACESO-main/
├── public/            # Static CSS, images, JS
├── views/             # EJS templates (index, login, register, secrets)
├── app.js             # Main server and routes
├── package.json
└── README.md
```

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/shreyawritescode/ACESO-main.git
   cd ACESO-main
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the root with:
   ```
   SECRET=your_secret_key
   ```
4. Ensure MongoDB is running locally on port 27017, then start the server:
   ```bash
   node app.js
   ```
5. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Routes

| Route | Method | Description |
|---|---|---|
| `/` | GET | Home page |
| `/login` | GET/POST | User login |
| `/register` | GET/POST | New user registration |
| `/secrets` | GET | Protected secrets page |
| `/logout` | GET | Logout |

---

*A Node.js authentication project exploring user management, password hashing, and session-based access control.*
