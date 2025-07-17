# MERN Stack Blog Application

A full-stack blog application built with MongoDB, Express.js, React.js, and Node.js for the PLP MERN Stack Development Course.

## 🚀 Features

- **User Authentication** - JWT-based registration and login
- **CRUD Operations** - Create, read, update, and delete blog posts
- **Category Management** - Organize posts by categories
- **Search & Filter** - Search posts and filter by category
- **Pagination** - Efficient data loading
- **Responsive Design** - Mobile-first design with Tailwind CSS
- **RESTful API** - Well-structured backend API

## 🛠️ Tech Stack

### Backend
- Node.js & Express.js
- MongoDB & Mongoose
- JWT Authentication
- Joi Validation
- Bcrypt for password hashing

### Frontend
- React 18
- React Router DOM
- Tailwind CSS
- Lucide React Icons
- React Hot Toast

## 📁 Project Structure

```
mern-blog/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # Reusable components
│   │   ├── pages/          # Page components
│   │   ├── context/        # React context
│   │   ├── services/       # API services
│   │   └── hooks/          # Custom hooks
│   └── package.json
├── server/                 # Express backend
│   ├── controllers/        # Route controllers
│   ├── models/             # Mongoose models
│   ├── routes/             # API routes
│   ├── middleware/         # Custom middleware
│   ├── utils/              # Utilities
│   └── package.json
└── README.md
```

## 🚀 Installation

### Prerequisites
- Node.js (v18+)
- MongoDB

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/PLP-MERN-Stack-Development/week-4-mern-integration-assignment-OneWilly.git
   cd week-4-mern-integration-assignment-OneWilly
   ```

2. **Server Setup**
   ```bash
   cd server
   npm install
   cp .env.example .env
   # Edit .env with your MongoDB URI and JWT secret
   npm run dev
   ```

3. **Client Setup**
   ```bash
   cd client
   npm install
   npm run dev
   ```

## 🔧 Environment Variables

### Server (.env)
```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/mern-blog
JWT_SECRET=your-jwt-secret-key
CLIENT_URL=http://localhost:5173
```

### Client (.env)
```
VITE_API_URL=http://localhost:5000/api
```

## 📚 API Endpoints

### Authentication
- `POST /api/auth/register` - Register user
- `POST /api/auth/login` - Login user
- `GET /api/auth/me` - Get current user

### Posts
- `GET /api/posts` - Get all posts (with pagination/search)
- `GET /api/posts/:id` - Get single post
- `POST /api/posts` - Create post (protected)
- `PUT /api/posts/:id` - Update post (protected)
- `DELETE /api/posts/:id` - Delete post (protected)

### Categories
- `GET /api/categories` - Get all categories
- `POST /api/categories` - Create category (protected)

## 🎯 Assignment Requirements

✅ **Task 1: Project Setup**
- MERN stack structure with client/server separation
- MongoDB integration with Mongoose
- Express.js API with proper middleware

✅ **Task 2: Backend Development**
- RESTful API endpoints
- User authentication with JWT
- Data validation with Joi
- Error handling middleware

✅ **Task 3: Frontend Development**
- React components and routing
- State management with Context API
- Custom hooks for API calls
- Responsive UI with Tailwind CSS

✅ **Task 4: Integration**
- API service layer
- Authentication flow
- CRUD operations
- Search and pagination

✅ **Task 5: Advanced Features**
- Protected routes
- Image upload support
- Category management
- User profiles

## 🚀 Usage

1. Start both server and client
2. Register a new account or login
3. Create, edit, and manage blog posts
4. Search and filter posts by category
5. Navigate through paginated results

## 👨‍💻 Author

**William Oneka**
- GitHub: [@OneWilly](https://github.com/OneWilly)
- Course: PLP MERN Stack Development
- Assignment: Week 4 MERN Integration
