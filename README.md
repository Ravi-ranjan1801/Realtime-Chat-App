# 💬 Real-time Chat Application

A modern, full-stack chat application built with the MERN stack, featuring real-time messaging, user authentication, and a sleek user interface.

![Chat App Demo](https://via.placeholder.com/800x400/4F46E5/FFFFFF?text=Real-time+Chat+App)

## ✨ Features

- 🔐 **Secure Authentication** - JWT-based user registration and login
- 💬 **Real-time Messaging** - Instant message delivery with Socket.io
- 👥 **Online Status** - See who's currently online
- 🎨 **Modern UI** - Beautiful, responsive design with TailwindCSS
- 📱 **Mobile Friendly** - Optimized for all device sizes
- 🖼️ **Media Sharing** - Upload and share images via Cloudinary
- ⚡ **Fast Performance** - Optimized with Zustand state management
- 🛡️ **Error Handling** - Comprehensive error handling on both client and server
- 🌙 **Dark Mode** - Toggle between light and dark themes

## 🚀 Tech Stack

### Frontend
- **React.js** - UI library
- **TailwindCSS** - Utility-first CSS framework
- **Daisy UI** - Beautiful component library
- **Zustand** - Lightweight state management
- **Socket.io Client** - Real-time communication

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - NoSQL database
- **Socket.io** - WebSocket library
- **JWT** - Authentication tokens
- **Bcrypt** - Password hashing

### Cloud Services
- **Cloudinary** - Image and media management
- **MongoDB Atlas** - Cloud database

## 📦 Installation

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- MongoDB Atlas account
- Cloudinary account

### Clone the Repository
```bash
git clone https://github.com/Ravi-ranjan1801/Realtime-Chat-App.git
cd Realtime-Chat-App
```

### Backend Setup
```bash
# Navigate to backend directory
cd backend

# Install dependencies
npm install

# Create .env file
cp .env.example .env
```

### Frontend Setup
```bash
# Navigate to frontend directory
cd frontend

# Install dependencies
npm install
```

## ⚙️ Environment Variables

Create a `.env` file in the backend directory:

```env
# Database
MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/chatapp

# JWT Secret
JWT_SECRET=your-super-secret-jwt-key

# Cloudinary Configuration
CLOUDINARY_CLOUD_NAME=your-cloud-name
CLOUDINARY_API_KEY=your-api-key
CLOUDINARY_API_SECRET=your-api-secret

# Server Configuration
PORT=5001
NODE_ENV=development
```

## 🏃‍♂️ Running the Application

### Development Mode

**Start Backend Server:**
```bash
cd backend
npm run dev
```

**Start Frontend Server:**
```bash
cd frontend
npm run dev
```

The application will be available at:
- Frontend: `http://localhost:3000`
- Backend: `http://localhost:5001`

### Production Mode
```bash
# Build frontend
cd frontend
npm run build

# Start production server
cd backend
npm start
```

## 📁 Project Structure

```
Realtime-Chat-App/
├── backend/
│   ├── controllers/
│   │   ├── auth.controller.js
│   │   └── message.controller.js
│   ├── middleware/
│   │   └── protectRoute.js
│   ├── models/
│   │   ├── user.model.js
│   │   └── message.model.js
│   ├── routes/
│   │   ├── auth.routes.js
│   │   └── message.routes.js
│   ├── socket/
│   │   └── socket.js
│   ├── utils/
│   │   └── generateToken.js
│   ├── server.js
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   ├── store/
│   │   ├── utils/
│   │   └── App.jsx
│   ├── public/
│   └── package.json
└── README.md
```

## 🔑 Key Features Implementation

### Authentication Flow
- User registration with email validation
- Secure password hashing with bcrypt
- JWT token generation and validation
- Protected routes middleware

### Real-time Messaging
- Socket.io integration for instant messaging
- Online user status tracking
- Message persistence in MongoDB
- Typing indicators

### State Management
- Zustand for global state management
- Optimistic UI updates
- Efficient re-rendering

## 🌐 API Endpoints

### Authentication
```
POST /api/auth/signup    - User registration
POST /api/auth/login     - User login
POST /api/auth/logout    - User logout
```

### Messages
```
GET  /api/messages/:id   - Get messages with user
POST /api/messages/send/:id - Send message to user
```

### Users
```
GET  /api/users          - Get all users for sidebar
```

## 🚀 Deployment

### Using Render (Recommended)

1. **Backend Deployment:**
   - Connect your GitHub repository
   - Set environment variables
   - Deploy with automatic builds

2. **Frontend Deployment:**
   - Create static site service
   - Connect repository
   - Set build command: `npm run build`

### Using Vercel + Railway

1. **Frontend on Vercel:**
   ```bash
   npm i -g vercel
   vercel --prod
   ```

2. **Backend on Railway:**
   - Connect GitHub repository
   - Add environment variables
   - Deploy automatically

## 🐛 Troubleshooting

### Common Issues

**CORS Errors:**
```javascript
// backend/server.js
app.use(cors({
  origin: ["http://localhost:3000", "your-frontend-url"],
  credentials: true
}));
```

**Socket.io Connection Issues:**
```javascript
// frontend/src/socket.js
const socket = io("your-backend-url", {
  autoConnect: false,
  withCredentials: true
});
```

**Environment Variables:**
- Ensure all required environment variables are set
- Check for typos in variable names
- Restart server after changing .env file

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Raviranjan Kumar**
- GitHub: [@Ravi-ranjan1801](https://github.com/Ravi-ranjan1801)
- LinkedIn: [Ravi Ranjan](https://www.linkedin.com/in/ravi-ranjan-687458280/)
- Email: raviranjan12059@gmail.com

## 🙏 Acknowledgments

- Socket.io for real-time communication
- TailwindCSS for beautiful styling
- MongoDB for reliable data storage
- Cloudinary for media management
- The open-source community for amazing tools

## 📈 Future Enhancements

- [ ] Group chat functionality
- [ ] Voice messages
- [ ] Video calling
- [ ] Message reactions
- [ ] File sharing
- [ ] Message search
- [ ] User profiles
- [ ] Chat themes
- [ ] Message encryption

---

⭐ If you found this project helpful, please give it a star on GitHub!

**Live Demo:** [Coming Soon](https://your-app-url.com)
