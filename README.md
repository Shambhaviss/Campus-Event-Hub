# Team_1_Group_1
# Campus Event Hub

## 📌 Project Overview

**Campus Event Hub** is a web-based event management platform designed to help students discover campus events and enable college administrators to manage event-related activities.

The project uses the MERN stack to provide a structured platform with role-based access for students, college administrators, and super administrators.

## 🎯 Objectives

- Provide a centralized platform for campus events.
- Organize events by category.
- Support role-based authentication and access.
- Allow administrators to manage college events.
- Store event and user information in a database.

## 🛠️ Technologies Used

### Frontend
- React.js
- Vite
- JavaScript
- HTML and CSS

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose, if used in the implementation
- REST APIs
- Multer for image uploads, if enabled in the current version

## ✨ Features

- **Role-based access:** Student, College Admin, and Super Admin roles.
- **Authentication:** Registration and login interfaces for administrators.
- **Event categories:** Technical, Cultural, Sports, and Workshops.
- **Event management:** Backend APIs for working with event information.
- **Image uploads:** Support for event images, if configured.
- **Database integration:** MongoDB storage for application data.
- **Admin dashboard:** Interface for administrative functionality.

*Features listed here should match the functionality currently implemented in the project.*

## 🏗️ Project Structure

The project is organized into frontend and backend components.

```text
Campus-Event-Hub/
├── campus-frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js
├── backend/
│   ├── package.json
│   └── server files
├── README.md
├── .gitignore
└── requirements.txt (not required for the JavaScript application)
```

Adjust this structure to match your actual repository folders.

## ⚙️ Getting Started

### Prerequisites

- Node.js and npm
- MongoDB
- Git

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_CLONE_URL
cd YOUR_PROJECT_FOLDER
```

Replace the placeholders with your actual GitHub clone URL and project folder name.

### 2. Set up the backend

Open a terminal in the backend directory and install dependencies:

```bash
npm install
```

Configure the required environment variables, such as the MongoDB connection string and any authentication secrets, according to the backend configuration.

Start the backend using the script defined in its `package.json`. For example:

```bash
npm start
```

### 3. Set up the frontend

Open another terminal in the frontend directory:

```bash
npm install
npm run dev
```

Open the local URL printed by Vite in the terminal.

### 4. Database configuration

Ensure MongoDB is running and that the backend uses the correct connection settings. The database name used during development was `campuseventhub`.

## 🔐 Security

- Keep database credentials, API keys, and authentication secrets in environment variables.
- Do not upload `.env` files or private credentials to GitHub.
- Configure authentication and authorization checks on the backend.

## 🔮 Future Improvements

- QR-code-based event attendance.
- Event participation certificates.
- Improved event search and filtering.
- Notifications and event reminders.
- Enhanced analytics for event participation.

## 👩‍💻 Project Type

Academic team project.

**Author:** Shambhavi Shrivastava

