# 🛒 E-Commerce Platform

A full-stack **eCommerce web application** built using the **MERN stack (MongoDB, Express.js, React.js, Node.js)**. The platform provides a complete online shopping experience with product discovery, cart management, user authentication, order tracking, reviews, payments, and an administrative dashboard.

## 🚀 Features

### 👤 User Features

* User registration and authentication
* Secure user profiles
* Product browsing and search
* Product reviews and ratings
* Product pagination
* Featured/top products carousel
* Shopping cart management
* Shipping and payment method selection
* Order placement and order history
* Order status tracking

### 🛠️ Admin Features

* Admin authentication
* Admin dashboard
* Product management — Add, Update & Delete
* User management
* Admin account management
* Order management
* Detailed order information
* Update order status to **Delivered**

### 💳 Payments & Services

* **Razorpay** payment gateway integration
* **Brevo SMTP** integration for email services
* MongoDB database with sample data seeding

---

## 🧰 Tech Stack

| Category        | Technologies                    |
| --------------- | ------------------------------- |
| Frontend        | React.js, JavaScript, HTML, CSS |
| Backend         | Node.js, Express.js             |
| Database        | MongoDB                         |
| Authentication  | JWT                             |
| Payments        | Razorpay                        |
| Email           | Brevo SMTP                      |
| Version Control | Git & GitHub                    |

---

## 📁 Project Structure

```text
E-Commerce-Platform/
│
├── backend/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   └── server.js
│
├── frontend/
│   ├── public/
│   └── src/
│       ├── components/
│       ├── pages/
│       ├── screens/
│       └── App.js
│
├── data/
├── .env.example
├── package.json
└── README.md
```

---

## 📥 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/E-Commerce-Platform.git
cd E-Commerce-Platform
```

### 2. Install Backend Dependencies

```bash
npm install
```

### 3. Install Frontend Dependencies

```bash
cd frontend
npm install
cd ..
```

---

## 🔐 Environment Variables

Create a `.env` file in the root directory:

```dotenv
NODE_ENV=development
PORT=5000

JWT_SECRET=ADD_YOUR_JWT_SECRET_HERE
MONGO_URI=ADD_YOUR_MONGO_URI_HERE

RAZORPAY_KEY_ID=ADD_YOUR_RAZORPAY_KEY_ID
RAZORPAY_KEY_SECRET=ADD_YOUR_RAZORPAY_KEY_SECRET

PAGINATION_MAX_LIMIT=12

EMAIL_HOST=smtp-relay.brevo.com
EMAIL_PORT=587
EMAIL_USER=ADD_YOUR_BREVO_LOGIN
EMAIL_PASS=ADD_YOUR_BREVO_PASSWORD
EMAIL_FROM=ADD_YOUR_BREVO_LOGIN
```

> ⚠️ Never commit your `.env` file or expose API keys, database credentials, JWT secrets, or payment credentials.

---

## ▶️ Run the Application

### Run Frontend & Backend Together

```bash
npm run dev
```

### Run Backend Only

```bash
npm run server
```

---

## 🗄️ Database Seeding

Import sample users and products:

```bash
npm run data:import
```

Destroy database data:

```bash
npm run data:destroy
```

> ⚠️ `data:destroy` permanently removes application data from the configured database.

---

## 🏗️ Production Build

Build the React frontend for production:

```bash
cd frontend
npm run build
```

---

## 🔄 Application Architecture

```text
                    ┌──────────────────┐
                    │   React.js UI    │
                    │    Frontend      │
                    └────────┬─────────┘
                             │
                             ▼
                    ┌──────────────────┐
                    │  Express.js API  │
                    │     Backend      │
                    └────────┬─────────┘
                             │
              ┌──────────────┼──────────────┐
              │              │              │
              ▼              ▼              ▼
        ┌──────────┐   ┌───────────┐  ┌────────────┐
        │ MongoDB  │   │ Razorpay  │  │ Brevo SMTP │
        │ Database │   │ Payments  │  │   Email    │
        └──────────┘   └───────────┘  └────────────┘
```

---

## 🤝 Contributing

Contributions are welcome.

### Create a Branch

```bash
git checkout -b feature/your-feature-name
```

For bug fixes:

```bash
git checkout -b fix/your-issue-name
```

### Commit Your Changes

```bash
git add .
git commit -m "Add your descriptive commit message"
```

### Push Your Changes

```bash
git push origin feature/your-feature-name
```

Then open a Pull Request on GitHub with a clear description of your changes.

---

## 📌 Future Improvements

* Product filtering and sorting
* Wishlist functionality
* Coupon and discount management
* Order cancellation and refunds
* Advanced analytics dashboard
* Image upload and cloud storage
* Automated testing
* CI/CD integration
* Enhanced mobile responsiveness

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

**Built with the MERN Stack 🚀**
