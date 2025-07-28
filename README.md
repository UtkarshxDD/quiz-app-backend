📝 Quiz Application - MERN Stack
A modern, full-featured quiz application built with the MERN stack (MongoDB, Express.js, React, Node.js) featuring a sleek tech-inspired dark theme.
Backend Github Rep : https://github.com/UtkarshxDD/quiz-app-backend/
🚀 Live Demo
Frontend: https://quiz-app-frontend-eight-eta.vercel.app/

Backend API: https://quiz-app-backend-2nnz.onrender.com/

✨ Features
Core Functionality
📧 Email-based Quiz Sessions - Users start with email authentication

⏰ 30-minute Timer - Countdown timer with auto-submit functionality

🎯 15 Dynamic Questions - Fetched from OpenTDB API

🧭 Question Navigation - Jump to any question with status tracking

📊 Detailed Results - Comprehensive answer comparison and scoring

🔄 Auto-submit - Quiz automatically submits when timer expires

User Experience
🎨 Modern Tech UI - Dark theme with neon green accents

📱 Fully Responsive - Works on desktop, tablet, and mobile

⚡ Real-time Updates - Question status and progress tracking

🎭 Smooth Animations - Enhanced user interactions

📈 Progress Analytics - Track attempted vs visited questions

Technical Features
🔒 Data Persistence - MongoDB stores quiz sessions and results

🌐 RESTful API - Clean API architecture

🎪 State Management - React Context for global state

🛡️ Error Handling - Comprehensive error management

📋 Input Validation - Frontend and backend validation

🛠️ Technology Stack
Frontend
React 18 - UI framework

React Context API - State management

Axios - HTTP client

CSS3 - Custom styling with modern design

Vercel - Deployment platform

Backend
Node.js - Runtime environment

Express.js - Web framework

MongoDB - Database

Mongoose - ODM for MongoDB

Render - Deployment platform

APIs
OpenTDB - Trivia questions database

🚀 Getting Started
Prerequisites
Node.js (v18 or higher)

MongoDB (local installation or MongoDB Atlas account)

Git

Installation
Clone the repository

text
git clone https://github.com/UtkarshxDD/quiz-app-backend/
cd quiz-app
Backend Setup

text
cd server
npm install
Frontend Setup

text
cd ../client
npm install
Environment Configuration

Create server/.env:

text
PORT=5000
MONGODB_URI=mongodb://localhost:27017/quizapp
NODE_ENV=development
FRONTEND_URL=http://localhost:3000
Create client/.env.local:

text
REACT_APP_API_URL=http://localhost:5000/api
Running the Application
Start Backend Server

text
cd server
npm run dev
Start Frontend (in a new terminal)

text
cd client
npm start
Access the Application

Frontend: http://localhost:3000

Backend API: http://localhost:5000

🌐 Deployment
Backend (Render)
Connect your GitHub repository to Render

Create a new Web Service with these settings:

Root Directory: server

Build Command: npm install

Start Command: npm start

Set environment variables in Render dashboard

Frontend (Vercel)
Connect your GitHub repository to Vercel

Configure deployment settings:

Root Directory: client

Build Command: npm run build

Output Directory: build

Set environment variables in Vercel dashboard

📡 API Endpoints
Quiz Management
POST /api/quiz/start - Start a new quiz session

PUT /api/quiz/question/:quizId/:questionId - Update question status

POST /api/quiz/submit/:quizId - Submit completed quiz

GET /api/quiz/results/:quizId - Retrieve quiz results

GET /api/health - Health check endpoint
