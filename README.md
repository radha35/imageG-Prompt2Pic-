# ImageZ - AI Powered Text-to-Image Generator

An AI-powered text-to-image generation platform built with the **MERN stack**. Users can register, log in, and generate high-quality AI images by entering a text prompt. Each account has a credits system that limits the number of images generated. Users can purchase more credits using **Razorpay** integration.  

🔗 **Live Demo:** [ImageZ Live](https://imagez-client.onrender.com/)  
📂 **Source Code:** [GitHub Repository](https://github.com/allknowledge34/ImageZ)

---

## 📜 Features
- 🔑 **User Authentication** with JWT (Signup/Login)
- 🖼 **AI Image Generation** using Clipdrop API
- 💳 **Credits System** - each generation deducts credits
- 🛒 **Subscription Plans** with Razorpay Payment Gateway
- 📱 **Responsive UI** built with React.js
- 🔒 Secure API & database integration
- 📦 MongoDB for data persistence

---

## 📂 Folder Structure
```
imageG/
│
├── client/       # React.js frontend
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── .env (hidden)
│
├── server/       # Node.js backend
│   ├── routes/
│   ├── models/
│   ├── controllers/
│   ├── server.js
│   ├── package.json
│   └── .env (hidden)
│
└── README.md
```

---

## 🛠 Tech Stack
**Frontend:** React.js, Axios, TailwindCSS  
**Backend:** Node.js, Express.js, JWT Authentication  
**Database:** MongoDB (Mongoose)  
**API:** Clipdrop API (AI image generation)  
**Payments:** Razorpay Integration  

---

## 🚀 Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/allknowledge34/ImageZ.git
cd ImageZ
```

### 2️⃣ Setup Backend (Server)
```bash
cd server
npm install
```

Create a `.env` file inside the `server` folder:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLIPDROP_API_KEY=your_clipdrop_api_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
```

Start the backend server:
```bash
npm start
```

---

### 3️⃣ Setup Frontend (Client)
Open a new terminal:
```bash
cd client
npm install
```

Create a `.env` file inside the `client` folder:
```env
VITE_BACKEND_URL=http://localhost:5000
VITE_RAZORPAY_KEY_ID=your_razorpay_key_id
```

Start the frontend:
```bash
npm run dev
```

---

## 📦 How to Run
1. Start **backend** (`server` folder)
2. Start **frontend** (`client` folder)
3. Open browser at: `http://localhost:5173` (default Vite port)

---

## 🔄 Flow Diagram
```plaintext
User (React.js Frontend) → [HTTPS Request] → Backend (Express.js)
→ MongoDB (Mongoose) → Clipdrop API (Image Generation)
→ Razorpay API (Payment Gateway) → Back to Frontend (UI Update)
```

---

## 📷 Screenshots
> *(Add your screenshots here for visual reference)*

---

## 💡 Subscription Plans
- ₹10 → 15 credits  
- ₹30 → 70 credits  
- ₹50 → 150 credits  

---

## 📜 License
This project is licensed under the **MIT License**.

---

## 👨‍💻 Author
**Radha**  
🔗 [GitHub](https://github.com/allknowledge34)  
