# imageG - AI Powered Text-to-Image Generator

An AI-powered text-to-image generation platform built with the **MERN stack**. Users can register, log in, and generate high-quality AI images by entering a text prompt. Each account has a credits system that limits the number of images generated. Users can purchase more credits using **Razorpay** integration.  

I built an AI-powered Text-to-Image Generator website using the MERN stack. After authentication via JWT, users can enter a text prompt, which is sent to the backend REST API in Node.js/Express. The backend calls the Clipdrop API with this prompt, which uses AI image generation models to create and return the image. Credits are deducted from MongoDB for each generation, and when credits run out, users can buy more through Razorpay integration. The frontend, built in React.js, provides a responsive and smooth user experience. This project gave me experience with API integration, AI image generation, payment gateways, and secure full-stack architecture.

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
git clone https://github.com/yourusername/imageG.git
cd imageG
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
> *(<img width="1919" height="921" alt="Screenshot 2025-08-11 203057" src="https://github.com/user-attachments/assets/78bdaa87-d8b5-4114-99b1-7cd4e653f807" />
<img width="1894" height="871" alt="Screenshot 2025-08-11 203117" src="https://github.com/user-attachments/assets/a9b41e6f-5d66-4a81-864e-e70e2c3435f3" />
<img width="1899" height="878" alt="Screenshot 2025-08-11 202954" src="https://github.com/user-attachments/assets/5c172274-881e-4570-94f7-2cf1dac4d13f" />
<img width="1919" height="871" alt="Screenshot 2025-08-11 203016" src="https://github.com/user-attachments/assets/2500a8a6-7eec-41c2-87d1-724127ccf8ea" />
<img width="1900" height="875" alt="Screenshot 2025-08-11 203039" src="https://github.com/user-attachments/assets/3cc6e542-b07f-48d7-a470-69f0fa0ded0c" />
<img width="1913" height="867" alt="Screenshot 2025-08-11 203317" src="https://github.com/user-attachments/assets/a817c93b-b22e-488b-b3de-1e96cb64f333" />
<img width="1887" height="876" alt="Screenshot 2025-08-11 203338" src="https://github.com/user-attachments/assets/fde68025-fea4-4bc8-87d1-96dbafb74715" />
<img width="1916" height="873" alt="Screenshot 2025-08-11 203414" src="https://github.com/user-attachments/assets/96149388-dcc9-49f2-a454-10a5c6550cef" />
)*

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
🔗 [GitHub](https://github.com/yourusername)  
