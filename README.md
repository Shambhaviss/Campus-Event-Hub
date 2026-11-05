# Team_1_Group_1
# Campus Event Hub

A full-stack web application designed to simplify campus event management by connecting students, college administrators, and platform administrators through a centralized platform.

Campus Event Hub provides features for event discovery, student registrations, QR-based attendance, notifications, certificates, and administrative management.

## Key Features

### User Management & Authentication
- Role-based access for Students, College Admins, and Super Admins.
- JWT-based authentication and protected routes.
- Google OAuth 2.0 integration.
- Secure password hashing using bcrypt.
- Forgot password and password reset functionality.
- College administrator approval workflow.

### Event Management
- Create, manage, and explore campus events.
- Organize events into categories such as Technical, Cultural, Sports, and Workshops.
- Manage event registrations.
- Upload and manage event images.

### Registration & Attendance
- Student event registration.
- QR code generation and scanning for attendance management.
- Registration tracking and administrative controls.

### Communication & Engagement
- Notifications for important activities.
- Event-related discussions and feedback.
- Email integration for account and administrative workflows.
- AI-powered chatbot integration.

### Administrative Dashboard
- Separate administrative functionality based on user roles.
- Manage users, events, and registrations.
- Review and approve college administrator accounts.
- Maintain administrative activity logs.

### Application Health & Diagnostics
- Database connectivity checks.
- User, event, and registration statistics.
- Service health status reporting.
- Manual health-check execution.
- API response-time and application uptime reporting.

## Technology Stack

| Layer | Technologies |
|---|---|
| Frontend | React.js, Vite, JavaScript |
| Styling | Tailwind CSS |
| Backend | Node.js, Express.js |
| Database | MongoDB, Mongoose |
| Authentication | JWT, Passport.js, Google OAuth 2.0 |
| Security | bcrypt, Helmet, CORS, express-rate-limit |
| API Communication | Axios |
| QR Functionality | qrcode, html5-qrcode |
| Data Visualization | Recharts |
| PDF & Excel Libraries | jsPDF, PDFKit, ExcelJS |
| Email | Nodemailer |
| AI Integration | Groq SDK, OpenAI SDK |
| Development Tools | Git, GitHub, ESLint, Nodemon |

## Project Architecture

The application follows a separate frontend and backend architecture.

```text
Campus-Event-Hub/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── assets/
│   │   └── ...
│   ├── package.json
│   └── vite.config.js
│
├── backend/
│   ├── src/
│   │   ├── config/
│   │   ├── controllers/
│   │   ├── middleware/
│   │   ├── models/
│   │   └── routes/
│   ├── server.js
│   └── package.json
│
└── README.md
```

*Note: The structure above illustrates the main organization; individual folders and filenames may vary.*

## Installation and Setup

### Prerequisites
- Node.js and npm
- MongoDB database
