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
git clone https://github.com/radha35/imageG-Prompt2Pic-.git
cd imageG
  
└── README.md
### 2️⃣ Setup Backend (Server)
```bash
cd server
npm install

