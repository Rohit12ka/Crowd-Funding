# 💰 Crowd-Funding Platform

A modern **Crowd-Funding Platform** that allows users to create fundraising campaigns and contribute funds to campaigns created by others. The platform provides an easy and transparent way for individuals or organizations to raise money for different causes, projects, and initiatives.

---

## 📌 Project Overview

The Crowd-Funding Platform is designed to connect **campaign creators** with **contributors**.

Users can:

- Create fundraising campaigns
- Add campaign details and funding goals
- Browse available campaigns
- Contribute to campaigns
- Track campaign progress
- View campaign information
- Manage their campaigns

The main goal of this project is to provide a simple and user-friendly platform for online fundraising.

---

## ✨ Features

### 👤 User Features

- User Registration & Login
- User Authentication
- User Profile Management
- Browse Campaigns
- Search Campaigns
- View Campaign Details
- Contribute to Campaigns
- Track Contribution History

### 📢 Campaign Features

- Create a New Campaign
- Add Campaign Title & Description
- Set Funding Goal
- Set Campaign Deadline
- Upload Campaign Image
- Display Amount Raised
- Display Funding Progress
- View Campaign Status
- Manage Created Campaigns

### 📊 Dashboard

Users can view:

- Total Campaigns
- Total Amount Raised
- Total Contributions
- Active Campaigns
- Completed Campaigns

---

## 🛠️ Technologies Used

### Frontend

- HTML5
- CSS3
- JavaScript
- React.js

### Backend

- Node.js
- Express.js

### Database

- MongoDB

### Other Technologies

- REST API
- Git & GitHub
- JWT Authentication
- Cloud/Local Image Storage

---

## 🏗️ Project Structure

```text
crowd-funding/
│
├── client/
│   ├── public/
│   └── src/
│       ├── components/
│       ├── pages/
│       ├── services/
│       ├── App.jsx
│       └── main.jsx
│
├── server/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   └── server.js
│
├── .gitignore
├── README.md
└── package.json
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/crowd-funding.git
```

### 2. Navigate to the Project

```bash
cd crowd-funding
```

### 3. Install Dependencies

For the frontend:

```bash
cd client
npm install
```

For the backend:

```bash
cd ../server
npm install
```

---

## 🔐 Environment Variables

Create a `.env` file inside the `server` directory.

```env
PORT=,,,,
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

Replace the values with your own configuration.

> ⚠️ Never upload your `.env` file or secret keys to GitHub.

---

## ▶️ Run the Project

### Start Backend

```bash
cd server
npm start
```

### Start Frontend

Open another terminal:

```bash
cd client
npm run dev
```

The application will then be available on the local development server.

---

## 🔄 Application Workflow

```text
User
  │
  ▼
Register / Login
  │
  ▼
Dashboard
  │
  ├───────────────┐
  ▼               ▼
Create Campaign   Browse Campaigns
  │               │
  ▼               ▼
Set Goal         Select Campaign
  │               │
  └───────┬───────┘
          ▼
       Contribute
          │
          ▼
   Campaign Progress
          │
          ▼
     Goal Reached
```

---

## 📸 Screenshots

Add screenshots of your project here.

### Home Page

```text
Add your screenshot here
```

### Campaign Page

```text
Add your screenshot here
```

### Dashboard

```text
Add your screenshot here
```

---

## 🎯 Use Cases

This platform can be used for:

- 🏥 Medical Fundraising
- 🎓 Education
- 🤝 Social Causes
- 🚀 Startup Projects
- 🎨 Creative Projects
- 🌱 Environmental Causes
- 🏘️ Community Projects
- ❤️ Personal Fundraising

---

## 🔒 Security

The application follows basic security practices such as:

- Password authentication
- JWT-based authorization
- Protected API routes
- Environment variables for sensitive information
- Input validation

---

## 🚀 Future Improvements

Some planned improvements include:

- Online Payment Gateway Integration
- Razorpay/Stripe Integration
- Campaign Verification
- Admin Dashboard
- Advanced Search & Filters
- Donation/Contribution Receipts
- Campaign Sharing on Social Media
- Real-time Campaign Updates

---

## 📚 Learning Outcomes

Through this project, I learned and practiced:

- Full-Stack Web Development
- REST API Development
- Database Management
- Authentication & Authorization
- CRUD Operations
- Frontend & Backend Integration
- Git & GitHub
- Responsive UI Development
- Deployment Concepts

---

## 👨‍💻 Author

**Dev Yadav**

- GitHub: [GitHub Profile](https://github.com/devbratyadav9792)

---

## 📄 License

This project is created for **educational and portfolio purposes**.

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.
