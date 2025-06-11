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

## 🚀 Deployment

### Deployment Options

#### 1. Render (Recommended)
1. Create a [Render](https://render.com) account
2. Create a new Web Service
3. Connect your GitHub repository
4. Configure the following settings:
   - **Build Command**: `npm install`
   - **Start Command**: `node app.js`
   - **Environment Variables**:
     ```
     MONGODB_URI=your_mongodb_connection_string
     JWT_SECRET=your_jwt_secret
     PORT=3000
     ```
5. Click "Create Web Service"

#### 2. Railway
1. Create a [Railway](https://railway.app) account
2. Create a new project
3. Connect your GitHub repository
4. Add the following environment variables:
   ```
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   PORT=3000
   ```
5. Railway will automatically detect your Node.js application and deploy it

#### 3. Heroku
1. Create a [Heroku](https://heroku.com) account
2. Install the Heroku CLI
3. Run the following commands:
   ```bash
   heroku login
   heroku create your-app-name
   heroku config:set MONGODB_URI=your_mongodb_connection_string
   heroku config:set JWT_SECRET=your_jwt_secret
   git push heroku main
   ```

### Pre-deployment Checklist

1. **Environment Variables**
   - Ensure all environment variables are properly set
   - Use strong, unique values for secrets
   - Never commit `.env` files to version control

2. **Database**
   - Set up a production MongoDB database (MongoDB Atlas recommended)
   - Update connection string with production credentials
   - Ensure database indexes are properly configured

3. **Security**
   - Enable HTTPS
   - Set secure cookie options
   - Configure CORS if needed
   - Set appropriate security headers

4. **Performance**
   - Enable compression
   - Configure caching where appropriate
   - Optimize static file serving

5. **Monitoring**
   - Set up error logging
   - Configure application monitoring
   - Set up uptime monitoring

### Post-deployment Steps

1. Test all features in the production environment
2. Monitor application logs for any errors
3. Set up automated backups for the database
4. Configure domain name and SSL certificate if needed
5. Set up CI/CD pipeline for future updates

### Troubleshooting Common Issues

1. **Application Crashes**
   - Check application logs
   - Verify environment variables
   - Ensure all dependencies are installed

2. **Database Connection Issues**
   - Verify MongoDB connection string
   - Check network access and firewall settings
   - Ensure database user has correct permissions

3. **File Upload Problems**
   - Verify storage permissions
   - Check file size limits
   - Ensure proper file type validation

For more detailed deployment instructions or specific platform requirements, please refer to the respective platform's documentation.

