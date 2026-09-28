# 🚀 Crowd-Funding Platform

A full-stack **Crowd-Funding Platform** that allows individuals, startups, organizations, and social initiatives to create fundraising campaigns and collect financial support from multiple contributors through a centralized platform.

The platform provides campaign management, user authentication, donation/contribution tracking, and transparent campaign information.

---

## 📌 Features

### 👤 User Features
- User Registration & Login
- Secure Authentication
- User Profile Management
- Browse Active Campaigns
- Search and Filter Campaigns
- View Campaign Details
- Contribute/Donate to Campaigns
- Track Contribution History

### 📢 Campaign Features
- Create a Fundraising Campaign
- Add Campaign Title & Description
- Set Funding Goal
- Set Campaign Deadline
- Upload Campaign Images
- Track Amount Raised
- Display Number of Contributors
- Campaign Progress Indicator
- Update Campaign Information
- Manage Created Campaigns

### 💰 Funding Features
- Make Contributions
- Contribution History
- Automatic Fund Progress Calculation
- Goal vs. Raised Amount Tracking
- Transaction Status
- Donor/Contributor Records

### 🔐 Security
- User Authentication
- Password Protection
- Input Validation
- Protected API Routes
- Secure Database Operations
- Authorization for Campaign Management

---

## 🛠️ Tech Stack

### Frontend
- React.js
- HTML5
- CSS3
- JavaScript
- Tailwind CSS / Bootstrap

### Backend
- Node.js
- Express.js

### Database
- MongoDB
- Mongoose

### Authentication
- JWT (JSON Web Token)
- bcrypt

### Payment Integration
- Razorpay / Stripe *(if implemented)*

### Development Tools
- Git
- GitHub
- VS Code
- Postman
- npm

---

## 🏗️ Project Architecture

```text
Crowd-Funding-Platform
│
├── client/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── context/
│   │   ├── assets/
│   │   └── App.jsx
│   │
│   └── package.json
│
├── server/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   ├── uploads/
│   ├── server.js
│   └── package.json
│
├── .env
├── .gitignore
└── README.md
```

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
Set Goal          Select Campaign
  │               │
  ▼               ▼
Publish           View Details
                  │
                  ▼
             Make Contribution
                  │
                  ▼
             Payment Gateway
                  │
                  ▼
            Transaction Success
                  │
                  ▼
          Campaign Amount Updated
```

---

## 🎯 Main Modules

### 1. Authentication Module

Users can create an account and log in securely.

Authentication can be implemented using:

```text
Register → Hash Password → Store User
Login → Verify Password → Generate JWT
```

---

### 2. Campaign Module

Campaign creators can:

- Create campaigns
- Set fundraising goals
- Add descriptions
- Upload images
- Set deadlines
- Monitor funding progress
- Manage their campaigns

Example:

```text
Campaign Goal:       ₹1,00,000
Amount Raised:       ₹65,000
Remaining Amount:    ₹35,000
Contributors:        120
Progress:            65%
```

---

### 3. Contribution Module

Users can select a campaign and contribute an amount.

Example:

```text
User → Select Campaign
     → Enter Amount
     → Payment
     → Transaction Verification
     → Contribution Recorded
     → Campaign Progress Updated
```

---

### 4. Dashboard

The dashboard provides an overview of:

- Total campaigns
- Active campaigns
- Completed campaigns
- Total funds raised
- User contributions
- Campaign performance

---

## 🗄️ Database Design

### User Collection

```text
User
├── _id
├── name
├── email
├── password
├── profileImage
├── role
└── createdAt
```

### Campaign Collection

```text
Campaign
├── _id
├── title
├── description
├── goalAmount
├── raisedAmount
├── image
├── category
├── creator
├── deadline
├── status
└── createdAt
```

### Contribution Collection

```text
Contribution
├── _id
├── user
├── campaign
├── amount
├── paymentId
├── status
└── createdAt
```

---

## 🔑 API Endpoints

### Authentication

```http
POST /api/auth/register
POST /api/auth/login
GET  /api/auth/profile
```

### Campaigns

```http
POST   /api/campaigns
GET    /api/campaigns
GET    /api/campaigns/:id
PUT    /api/campaigns/:id
DELETE /api/campaigns/:id
```

### Contributions

```http
POST /api/contributions
GET  /api/contributions
GET  /api/contributions/:id
```

---

## ⚙️ Installation

### 1. Clone Repository

```bash
git clone https://github.com/yourusername/crowd-funding-platform.git
```

### 2. Navigate to Project

```bash
cd crowd-funding-platform
```

### 3. Install Frontend Dependencies

```bash
cd client
npm install
```

### 4. Install Backend Dependencies

```bash
cd ../server
npm install
```

---

## 🔐 Environment Variables

Create a `.env` file inside the `server` directory.

```env
PORT=5000

MONGO_URI=your_mongodb_connection_string

JWT_SECRET=your_jwt_secret

RAZORPAY_KEY_ID=your_razorpay_key
RAZORPAY_KEY_SECRET=your_razorpay_secret
```

> Never upload your `.env` file or API/payment credentials to GitHub.

---

## ▶️ Running the Project

### Start Backend

```bash
cd server
npm run dev
```

### Start Frontend

Open another terminal:

```bash
cd client
npm run dev
```

The application will normally be available at:

```text
Frontend: http://localhost:5173
Backend:  http://localhost:5000
```

---

## 🧪 Testing

API testing can be performed using **Postman**.

Test the following:

- User Registration
- User Login
- Campaign Creation
- Campaign Retrieval
- Campaign Update
- Campaign Deletion
- Contribution
- Payment Verification
- Authentication
- Authorization

---

## 🔒 Security Considerations

The application should follow these security practices:

- Hash passwords using bcrypt
- Use JWT for authentication
- Validate user input
- Protect private API routes
- Verify payment transactions on the server
- Store secrets in environment variables
- Prevent unauthorized campaign modification
- Sanitize database inputs

---

## 📊 Future Enhancements

The platform can be extended with:

- 🔔 Email Notifications
- 📱 SMS Notifications
- 💳 Multiple Payment Gateways
- 🏦 Automatic Fund Settlement
- 📈 Advanced Campaign Analytics
- ⭐ Campaign Reviews & Ratings
- ❤️ Campaign Wishlist
- 🔍 Advanced Search & Filtering
- 🌐 Multi-language Support
- 📱 Mobile Application
- 🛡️ Fraud Detection
- 🤖 AI-based Campaign Verification
- 🔗 Blockchain-based Transaction Transparency
- 📊 Admin Analytics Dashboard

---

## 🌟 Future Vision

The goal of this project is to create a transparent and scalable crowdfunding ecosystem where campaign creators can raise funds while contributors can easily discover and support projects they care about.

The platform can eventually support:

```text
Creators
    ↓
Campaign Platform
    ↓
Verification
    ↓
Contributors
    ↓
Secure Payments
    ↓
Transparent Fund Tracking
```

---

## 👨‍💻 Author

**Your Name**

GitHub: `https://github.com/yourusername`

LinkedIn: `https://linkedin.com/in/yourusername`

---

## 📄 License

This project is developed for educational and demonstration purposes.

You can add an MIT License if you intend to distribute the project under that license.

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.
