# MyBlog 📝

A modern blog platform built with Node.js and Express.js that allows users to create, manage, and interact with blog posts. The platform features user authentication, profile management, and social interactions through likes.

## ✨ Features

- **User Authentication**
  - Secure registration and login system
  - JWT-based authentication
  - Password encryption using bcrypt
  - Session management

- **Blog Management**
  - Create new blog posts
  - Edit existing posts
  - Delete posts
  - View all posts
  - Like and unlike posts

- **User Profile**
  - Profile picture upload
  - Profile information management
  - Personalized greeting on login

## 🛠️ Tech Stack

- **Backend**
  - Node.js
  - Express.js
  - MongoDB (Database)
  - Mongoose (ODM)

- **Authentication & Security**
  - JWT (JSON Web Tokens)
  - bcryptjs (Password Hashing)
  - Cookie Parser

- **File Handling**
  - Multer (File Upload)

- **View Engine**
  - EJS (Embedded JavaScript)

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- MongoDB
- npm or yarn

### Installation

1. Clone the repository
   ```bash
   git clone <repository-url>
   cd MyBlog
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Set up environment variables
   Create a `.env` file in the root directory and add:
   ```
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   PORT=3000
   ```

4. Start the server
   ```bash
   npm start
   ```

5. Open your browser and navigate to `http://localhost:3000`

## 📁 Project Structure

```
MyBlog/
├── models/         # Database models
├── views/          # EJS templates
├── public/         # Static files
├── utils/          # Utility functions
├── app.js          # Main application file
└── package.json    # Project dependencies
```

## 🔒 Security Features

- Password hashing using bcrypt
- JWT-based authentication
- Secure cookie handling
- Protected routes
- File upload validation

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the ISC License.

