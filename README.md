# 💬 Real-time Chat Application

<div align="center">

![Chat Application](https://img.shields.io/badge/Chat-Application-blue?style=for-the-badge)
![MERN Stack](https://img.shields.io/badge/MERN-Stack-green?style=for-the-badge)
![Socket.io](https://img.shields.io/badge/Socket.io-Real--time-orange?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

**A modern, full-stack chat application built with the MERN stack, featuring real-time messaging, user authentication, and a sleek user interface.**

[🚀 Live Demo](https://your-app-url.com) • [📖 Documentation](#) • [🐛 Report Bug](https://github.com/Ravi-ranjan1801/Realtime-Chat-App/issues) • [✨ Request Feature](https://github.com/Ravi-ranjan1801/Realtime-Chat-App/issues)

</div>

---

## 📸 Screenshots

<div align="center">
  <img src="https://via.placeholder.com/800x400/667eea/ffffff?text=Chat+Interface" alt="Chat Interface" style="border-radius: 10px; margin: 10px;"/>
  <img src="https://via.placeholder.com/400x300/764ba2/ffffff?text=Login+Screen" alt="Login Screen" style="border-radius: 10px; margin: 10px;"/>
  <img src="https://via.placeholder.com/400x300/f093fb/ffffff?text=Mobile+View" alt="Mobile View" style="border-radius: 10px; margin: 10px;"/>
</div>

---

## ✨ Features

<table>
<tr>
<td width="50%">

### 🔐 **Authentication & Security**
- JWT-based secure authentication
- Password hashing with bcrypt
- Protected routes and middleware
- Session management

### 💬 **Real-time Communication**
- Instant message delivery
- WebSocket connections
- Online/offline status tracking
- Typing indicators

</td>
<td width="50%">

### 🎨 **Modern UI/UX**
- Beautiful, responsive design
- Dark/Light theme toggle
- Mobile-optimized interface
- Smooth animations

### ⚡ **Performance & Features**
- Image upload and sharing
- Optimized state management
- Error handling & validation
- Cross-platform compatibility

</td>
</tr>
</table>

---

## 🛠️ Tech Stack

<div align="center">

### Frontend
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Socket.io](https://img.shields.io/badge/Socket.io-black?style=for-the-badge&logo=socket.io&badgeColor=010101)

### Backend
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-404D59?style=for-the-badge)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)

### Cloud & Tools
![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)

</div>

---

## 🚀 Quick Start

### Prerequisites

<table>
<tr>
<td>

```bash
# Check Node.js version
node --version
# Should be v14 or higher
```

</td>
<td>

```bash
# Check npm version  
npm --version
# Latest version recommended
```

</td>
</tr>
</table>

### 📦 Installation

```bash
# 1️⃣ Clone the repository
git clone https://github.com/Ravi-ranjan1801/Realtime-Chat-App.git
cd Realtime-Chat-App

# 2️⃣ Install backend dependencies
cd backend
npm install

# 3️⃣ Install frontend dependencies
cd ../frontend
npm install

# 4️⃣ Set up environment variables
cd ../backend
cp .env.example .env
# Edit .env with your configuration
```

### ⚙️ Environment Configuration

Create a `.env` file in the backend directory:

```env
# 🗄️ Database Configuration
MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/chatapp

# 🔐 JWT Configuration
JWT_SECRET=your-super-secret-jwt-key-make-it-long-and-secure

# ☁️ Cloudinary Configuration
CLOUDINARY_CLOUD_NAME=your-cloud-name
CLOUDINARY_API_KEY=your-api-key
CLOUDINARY_API_SECRET=your-api-secret

# 🚀 Server Configuration
PORT=5001
NODE_ENV=development
```

### 🏃‍♂️ Running the Application

<table>
<tr>
<td width="50%">

**🔧 Development Mode**
```bash
# Terminal 1: Start Backend
cd backend
npm run dev

# Terminal 2: Start Frontend  
cd frontend
npm run dev
```

</td>
<td width="50%">

**🚀 Production Mode**
```bash
# Build frontend
cd frontend
npm run build

# Start production server
cd ../backend
npm start
```

</td>
</tr>
</table>

<div align="center">

**🎉 Your app will be running at:**
- **Frontend:** `http://localhost:3000`
- **Backend:** `http://localhost:5001`

</div>

---

## 📁 Project Structure

```
📦 Realtime-Chat-App
├── 🔧 backend/
│   ├── 🎮 controllers/
│   │   ├── auth.controller.js
│   │   ├── message.controller.js
│   │   └── user.controller.js
│   ├── 🛡️ middleware/
│   │   └── protectRoute.js
│   ├── 📊 models/
│   │   ├── user.model.js
│   │   └── message.model.js
│   ├── 🛣️ routes/
│   │   ├── auth.routes.js
│   │   ├── message.routes.js
│   │   └── user.routes.js
│   ├── 🔌 socket/
│   │   └── socket.js
│   ├── 🛠️ utils/
│   │   ├── generateToken.js
│   │   └── cloudinary.js
│   ├── 🚀 server.js
│   └── 📋 package.json
├── 🎨 frontend/
│   ├── src/
│   │   ├── 🧩 components/
│   │   ├── 📄 pages/
│   │   ├── 🪝 hooks/
│   │   ├── 🗃️ store/
│   │   ├── 🛠️ utils/
│   │   └── 📱 App.jsx
│   ├── 🌐 public/
│   └── 📋 package.json
└── 📖 README.md
```

---

## 🔗 API Endpoints

<div align="center">

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| `POST` | `/api/auth/signup` | User registration | ❌ |
| `POST` | `/api/auth/login` | User login | ❌ |
| `POST` | `/api/auth/logout` | User logout | ✅ |
| `GET` | `/api/messages/:id` | Get chat messages | ✅ |
| `POST` | `/api/messages/send/:id` | Send message | ✅ |
| `GET` | `/api/users` | Get all users | ✅ |

</div>

---

## 🌐 Deployment Guide

<div align="center">

### 🆓 Free Deployment Options

</div>

<table>
<tr>
<td width="33%">

### 🟦 **Render**
```bash
# Backend & Frontend
✅ Free tier available
✅ Auto-deploy from Git
✅ Built-in SSL
✅ Environment variables
```

</td>
<td width="33%">

### ⚡ **Vercel + Railway**
```bash
# Frontend: Vercel
# Backend: Railway
✅ Excellent performance
✅ Global CDN
✅ Easy setup
```

</td>
<td width="33%">

### 🟢 **Netlify + Heroku**
```bash
# Frontend: Netlify  
# Backend: Heroku
✅ Popular choice
✅ Good documentation
✅ CI/CD integration
```

</td>
</tr>
</table>

### 🔧 Deployment Steps

1. **Prepare Environment Variables**
2. **Build the Application**
3. **Deploy Backend Service**
4. **Deploy Frontend Application**
5. **Configure Domain (Optional)**

> 📚 **Detailed deployment guide:** [View Documentation](#)

---

## 🐛 Troubleshooting

<details>
<summary><strong>🔴 Common Issues & Solutions</strong></summary>

### CORS Errors
```javascript
// backend/server.js
app.use(cors({
  origin: ["http://localhost:3000", "your-frontend-url"],
  credentials: true
}));
```

### Socket.io Connection Issues  
```javascript
// frontend/src/socket.js
const socket = io("your-backend-url", {
  autoConnect: false,
  withCredentials: true
});
```

### Environment Variables Not Loading
- ✅ Check `.env` file location
- ✅ Restart development server
- ✅ Verify variable names
- ✅ No spaces around `=` sign

</details>

---

## 🤝 Contributing

<div align="center">

We love contributions! Here's how you can help make this project better:

</div>

```bash
# 1️⃣ Fork the repository
# 2️⃣ Create your feature branch
git checkout -b feature/AmazingFeature

# 3️⃣ Commit your changes  
git commit -m 'Add some AmazingFeature'

# 4️⃣ Push to the branch
git push origin feature/AmazingFeature

# 5️⃣ Open a Pull Request
```

### 📋 Contribution Guidelines
- Follow existing code style
- Add tests for new features
- Update documentation
- Create detailed PR descriptions

---

## 📜 License

<div align="center">

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

</div>

---

## 👨‍💻 Author

<div align="center">

<img src="https://avatars.githubusercontent.com/u/yourusername?v=4" width="100" height="100" style="border-radius: 50%;" alt="Raviranjan Kumar"/>

### **Raviranjan Kumar**
*Full Stack Developer & Student*

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Ravi-ranjan1801)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ravi-ranjan-687458280/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:raviranjan12059@gmail.com)

</div>

---

## 🙏 Acknowledgments

<div align="center">

Special thanks to the amazing open-source community and these fantastic tools:

![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=for-the-badge&logo=socket.io&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)
![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white)

</div>

---

## 🚀 Future Enhancements

<div align="center">

| Feature | Status | Priority |
|---------|--------|----------|
| 👥 Group Chat | 🔄 In Progress | High |
| 🎵 Voice Messages | 📋 Planned | Medium |
| 📹 Video Calling | 🔮 Future | High |
| 👍 Message Reactions | 📋 Planned | Low |
| 📎 File Sharing | 🔮 Future | Medium |
| 🔍 Message Search | 📋 Planned | Medium |
| 👤 User Profiles | 🔄 In Progress | Low |
| 🎨 Chat Themes | 🔮 Future | Low |
| 🔐 End-to-End Encryption | 🔮 Future | High |

</div>

---

<div align="center">

### ⭐ Star this repository if you found it helpful!

![Stars](https://img.shields.io/github/stars/Ravi-ranjan1801/Realtime-Chat-App?style=social)
![Forks](https://img.shields.io/github/forks/Ravi-ranjan1801/Realtime-Chat-App?style=social)
![Issues](https://img.shields.io/github/issues/Ravi-ranjan1801/Realtime-Chat-App?style=social)

**Made with ❤️ by [Raviranjan Kumar](https://github.com/Ravi-ranjan1801)**

</div>
