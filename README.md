# EchoRoom
🎙️ EchoRoom

A Structured Debate & Opinion Platform

EchoRoom is a full-stack web application that enables users to participate in structured debates, share opinions, and engage in meaningful discussions. The platform integrates AI-powered tools and built-in moderation to ensure high-quality and safe interactions.


📌 Overview

EchoRoom is designed to solve the problem of unstructured and chaotic online discussions by introducing:

Organized debate topics
Clear For / Against opinion structure
Controlled moderation workflow
AI-assisted argument support

Users can explore debates, contribute opinions, vote, reply, and interact in a structured environment.


✨ Key Features

👤 User Features

User Registration & Login
JWT Authentication
Google Sign-In
Profile Management
View personal activity

💬 Debate System

Browse approved categories & topics
Create debate topics (approval-based)
Post opinions (For / Against)
Reply to opinions (single-level)
Vote on opinions
Report inappropriate content

🛠️ Admin Features

Approve / Reject categories & topics
Moderate opinions
Manage users (ban / suspend)
View system statistics

🤖 AI Features

Generate arguments
Enhance writing
Summarize debate topics
Chat-based assistance

🛠️ Tech Stack

Backend

Django 6
Django REST Framework
SimpleJWT
PostgreSQL (Production) / SQLite (Development)
Gunicorn, WhiteNoise
boto3
vaderSentiment

Frontend

React 19
Vite
React Router
Google OAuth
ESLint


## 📁 Project Structure  

```bash
EchoRoom/
│
├── public/
│   ├── favicon.ico
│   ├── index.html
│   ├── logo192.png
│   ├── logo512.png
│   ├── manifest.json
│   └── robots.txt
│
├── src/
│   ├── components/
│   │   └── navbar.jsx
│   │
│   ├── pages/
│   │   ├── Home.jsx
│   │   ├── Debate.jsx
│   │   ├── Category.jsx
│   │   ├── Admin.jsx
│   │   ├── Login.jsx
│   │   └── Register.jsx
│   │
│   ├── App.jsx
│   ├── App.test.jsx
│   ├── index.jsx
│   ├── index.css
│   └── styles.css
│
├── package.json
├── package-lock.json
├── README.md
└── .gitignore
```


⚙️ Installation & Setup

  Clone the repository

    git clone https://github.com/your-username/EchoRoom.git

  Navigate into the project folder

    cd EchoRoom

  Install dependencies

    npm install

  Start the development server

    npm start

  The application will run on:

    http://localhost:3000



📌 Current Status

  Frontend(in-process)

  Mock data used for debates, opinions, and admin panel

  No backend integration yet

  Authentication is simulated

🎯 Future Improvements

  Backend integration 

  Real authentication & database

  Real-time updates

  Improved search functionality

  User profile pages



👩‍💻 Developed By

Manushri : 202512122

Ruchita  : 202512070

Rishika  : 202512041

Krisha   : 202512112
