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

->Backend

Django 6

Django REST Framework

SimpleJWT

PostgreSQL (Production) / SQLite (Development)

Gunicorn, WhiteNoise

boto3

vaderSentiment



->Frontend

React 19

Vite

React Router

Google OAuth

ESLint


## 📁 Project Structure  

```bash
EchoRoom/
│
├── backend/
│   ├── echoroom/         
│   ├── accounts/          
│   ├── debates/           
│   ├── admin_api/        
│   ├── manage.py
│   ├── requirements.txt
│   ├── db.sqlite3        
│   └── .env              
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


🧠 Core Concepts

User → Custom model with roles, ban/suspend system

Category → Approval-based visibility

DebateTopic → Moderated before publishing

Opinion → For/Against stance with sentiment & toxicity analysis

Vote → One vote per user per opinion

Report → Moderation flag system

🔄 Main User Flows

🌐 Public Users

View categories & topics

Read opinions

👤 Registered Users

Create topics & categories

Post opinions & replies

Vote & report

Manage profile

🛡️ Admin

Approve/reject content

Moderate users & opinions

Monitor platform activity


🔌 API Overview

🔐 Authentication

POST /api/token/

POST /api/token/refresh/

POST /api/auth/register/

GET /api/auth/me/

POST /api/social/google/


💬 Debate APIs

GET /api/debates/categories/

GET /api/debates/topics/

POST /api/debates/topics/create/

POST /api/debates/opinions/...


🤖 AI APIs

Generate / Enhance Argument

Topic Summary

Chat Assistance


🛠️ Admin APIs

Manage topics, users, categories

Moderation endpoints



⚙️ Local Setup

->Backend Setup

cd backend

python -m venv .venv

.venv\Scripts\activate

pip install -r requirements.txt

python manage.py migrate

python manage.py loaddata db_seed_utf8.json

python manage.py runserver

->Frontend Setup

cd frontend

npm install

npm run dev


🔐 Authentication

JWT-based authentication

Access + Refresh tokens

Google OAuth integration

Token stored in frontend local storage


🛡️ Moderation System

Topics & categories require approval

Opinions can be reported

Admins can ban/suspend users

Automatic enforcement of user status


🤖 AI Integration

EchoRoom integrates AI to:

Generate arguments

Improve writing quality

Summarize discussions

Provide chat-based assistance



🚀 Future Improvements

Implement real-time updates & notifications

Enhance AI features for better accuracy

Improve UI/UX and responsiveness

Add search and recommendation system



🌐 Live Demo

👉 https://echoroom-frontend-v3.onrender.com/
