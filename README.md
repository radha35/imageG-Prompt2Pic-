# ImageG- AI Powered Text-to-Image Generator

I built an AI-powered Text-to-Image Generator website using the MERN stack. After authentication via JWT, users can enter a text prompt, which is sent to the backend REST API in Node.js/Express. The backend calls the Clipdrop API with this prompt, which uses AI image generation models to create and return the image. Credits are deducted from MongoDB for each generation, and when credits run out, users can buy more through Razorpay integration. The frontend, built in React.js, provides a responsive and smooth user experience. This project gave me experience with API integration, AI image generation, payment gateways, and secure full-stack architecture

🔗 **Live Demo:** [ImageZ Live](https://imagez-client.onrender.com/)  
📂 **Source Code:** [GitHub Repository](https://github.com/radha35/imageG-Prompt2Pic-)

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
imageG/
│
├── client/ # React.js frontend
│ ├── src/
│ ├── public/
│ ├── package.json
│ └── .env (hidden)
│
├── server/ # Node.js backend
│ ├── routes/
│ ├── models/
│ ├── controllers/
│ ├── server.js
│ ├── package.json
│ └── .env (hidden)
│


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
  
└── README.md

2️⃣ Setup Backend (Server)
bash
Copy
Edit
cd server
npm install
Create a .env file inside the server folder:

env
Copy
Edit
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
CLIPDROP_API_KEY=your_clipdrop_api_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
Start the backend server:

bash
Copy
Edit
npm start
3️⃣ Setup Frontend (Client)
Open a new terminal:

bash
Copy
Edit
cd client
npm install
Create a .env file inside the client folder:

env
Copy
Edit
VITE_BACKEND_URL=http://localhost:5000
VITE_RAZORPAY_KEY_ID=your_razorpay_key_id
Start the frontend:

bash
Copy
Edit
npm run dev
📦 How to Run
Start backend (server folder)

Start frontend (client folder)

Open browser at: http://localhost:5173 (default Vite port)

🔄 Flow Diagram
plaintext
Copy
Edit
User (React.js Frontend) → [HTTPS Request] → Backend (Express.js)
→ MongoDB (Mongoose) → Clipdrop API (Image Generation)
→ Razorpay API (Payment Gateway) → Back to Frontend (UI Update)
