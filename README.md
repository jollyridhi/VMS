
# 🛂 Enterprise Visitor Access Suite

A full-stack Enterprise Visitor Access Suite built to streamline guest check-ins, maintain visitor logs, and enhance security. The platform includes both backend REST APIs and a user-friendly frontend, ideal for offices, startups, or event venues.

---

## 📌 Features

- 🔐 **Secure Authentication** – Admin login for managing visitor data
- 🧾 **Visitor Registration** – Capture visitor name, contact, host, purpose, and more
- 🕒 **Check-in/Check-out System** – Real-time tracking of visitor status
- 📄 **Visitor Logs** – Maintain searchable records with timestamps
- 📧 **Email Notifications** – Send visit confirmation to hosts/visitors (optional)
- 📊 **Dashboard** – Admin view with all current and past visitors
- 🔎 **Search & Filter** – Easily find past visits using filters

---

## 💻 Tech Stack

| Layer        | Technology             |
|--------------|------------------------|
| Frontend     | React.js, Tailwind CSS |
| Backend      | Node.js, Express.js    |
| Database     | MongoDB (Mongoose)     |
| Auth         | JWT-based Auth         |
| Deployment   | Vercel (Frontend), Render (Backend) |

---

## 📁 Project Structure

```
/client               --> React Frontend
  └── /src
       ├── /components
       ├── /pages
       ├── /utils
       └── App.js

/server               --> Node.js Backend
  ├── /controllers
  ├── /models
  ├── /routes
  ├── /middleware
  └── server.js

.env.example          --> Sample env variables
README.md
```

---

## 🚀 Getting Started

### Prerequisites

- Node.js
- MongoDB Atlas or Local Mongo instance

### Installation

```bash
# Clone the repo
git clone https://github.com/jollyridhi/Enterprise-Visitor-Access-Suite.git
cd Enterprise-Visitor-Access-Suite

# Install backend dependencies
cd server
npm install

# Install frontend dependencies
cd ../client
npm install
```

### Environment Setup

Create a `.env` file in `/server`:

```env
PORT=5000
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_jwt_secret
```

---

### Running the App

```bash
# Run backend
cd server
npm run dev

# Run frontend
cd ../client
npm start
```

---

## 🔐 Authentication

- Admins can log in using registered credentials.
- Uses **JWT Tokens** to protect private routes.
- Middleware checks auth before allowing access to sensitive operations.

---

## 🧪 Testing (Optional)

- **Postman** used for API testing
- Sample collection file: `/docs/postman_collection.json`
- UI tests can be added using **Jest + React Testing Library**

---

## 🧩 Possible Improvements

- Add SMS/Email OTP verification
- Implement visitor photo upload
- Export logs to Excel or PDF
- Add role-based access (e.g., security, admin)

---

## 📸 UI Screenshots

> Add screenshots here using:
```
![Dashboard](screenshots/dashboard.png)
![Login](screenshots/login.png)
```

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

---

## 📄 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.

---

## 🙋‍♂️ Maintainer

Built with 💻 by [Ridhi Jolly](https://github.com/jollyridhi)
