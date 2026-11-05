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
- Git

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd Campus-Event-Hub
```

### 2. Set Up the Backend

```bash
cd backend
npm install
```

Create a `.env` file in the backend directory and configure the required environment variables:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
FRONTEND_URL=http://localhost:5173
```

Additional environment variables may be required for Google OAuth, email services, and AI integrations depending on the features you configure.

Start the backend:

```bash
npm run dev
```

### 3. Set Up the Frontend

Open another terminal:

```bash
cd frontend
npm install
npm run dev
```

Open the local URL displayed by Vite, usually:

```text
http://localhost:5173
```

## API Overview

The backend exposes modular API route groups, including:

| Endpoint | Purpose |
|---|---|
| `/api/auth` | Authentication and account management |
| `/api/users` | User management |
| `/api/admin` | Administrative operations |
| `/api/events` | Event management |
| `/api/registrations` | Event registrations |
| `/api/notifications` | Notifications |
| `/api/discussions` | Event discussions |
| `/api/certificates` | Certificate operations |
| `/api/feedback` | Feedback management |
| `/api/admin-logs` | Administrative audit logs |
| `/api/health` | Application health and diagnostics |

Most administrative operations are protected by authentication and role-based authorization.

## Security Measures

- JWT-based authentication and protected API routes.
- Role-based access control.
- Password hashing with bcrypt.
- Login and registration rate limiting.
- Helmet security headers.
- CORS configuration.
- Request-body sanitization.
- Cryptographically generated password-reset tokens with expiry.
- Environment variables for sensitive configuration.

## Development

Backend development:

```bash
npm run dev
```

Frontend development:

```bash
npm run dev
```

Frontend production build:

```bash
npm run build
```

Frontend linting:

```bash
npm run lint
```

## Project Objective

Campus Event Hub aims to make college event coordination more organized and accessible by providing a centralized platform for students and administrators. It combines full-stack web development, database management, authentication, API integration, and administrative workflows in one application.

## Future Enhancements

- Cloud deployment and scalable infrastructure.
- Automated testing and CI/CD integration.
- Advanced analytics and reporting.
- Enhanced monitoring and performance optimization.
