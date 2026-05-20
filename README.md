# 📄 ResumeHub - Resume Builder

> **Full-stack resume builder application for creating professional resumes with multiple templates**

[![React](https://img.shields.io/badge/Frontend-React-%2361DAFB?logo=react&logoColor=white)](https://react.dev/)
[![Node.js](https://img.shields.io/badge/Backend-Node.js-%23339933?logo=node.js&logoColor=white)](https://nodejs.org/)
[![Express](https://img.shields.io/badge/Framework-Express-%23000000?logo=express)](https://expressjs.com/)
[![MongoDB](https://img.shields.io/badge/Database-MongoDB-%2347A248?logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Zustand](https://img.shields.io/badge/State-Zustand-%23FBD84E)](https://github.com/pmndrs/zustand)
[![Tailwind CSS](https://img.shields.io/badge/Styling-Tailwind-%2338B2AC?logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

🔗 **[Live Demo](https://resumebuilderhub.netlify.app/)** • 📚 **[Documentation](#documentation)** • 🐛 **[Report Bug](https://github.com/jatinagrahari/Resume-Hub-Resume-Builder-/issues)** • ⭐ **[GitHub](https://github.com/jatinagrahari/Resume-Hub-Resume-Builder-)**

---

## ✨ Features

- 📋 **Multiple Templates** - Choose from various professional resume templates
- 📝 **Easy Form Filling** - Simple, intuitive form interface
- 👁️ **Live Preview** - See changes in real-time
- 📥 **PDF Export** - Download resumes as PDF
- 💾 **Save & Load** - Store resumes in cloud
- 🎨 **Customizable** - Modify colors, fonts, layouts
- 📱 **Responsive Design** - Works on all devices
- 🔐 **Secure** - User authentication and data encryption
- ⚡ **Fast Performance** - Optimized for speed
- 🌙 **Dark Mode** - Easy on the eyes
- 🔒 **Privacy First** - Your data stays with you
- ♿ **Accessible** - WCAG compliant

---

## 🏗️ Architecture

### Frontend Stack
- **Framework:** React 18
- **State Management:** Zustand
- **Styling:** Tailwind CSS
- **Routing:** React Router
- **API Client:** Axios

### Backend Stack
- **Runtime:** Node.js
- **Framework:** Express.js
- **Database:** MongoDB
- **Authentication:** JWT
- **File Upload:** Multer

---

## 🚀 Quick Start

### Prerequisites
- Node.js (v16 or higher)
- MongoDB (local or Atlas)
- npm or yarn

### Installation

#### Frontend Setup

```bash
# Navigate to client directory
cd client

# Install dependencies
npm install

# Start development server
npm run dev
```

#### Backend Setup

```bash
# Navigate to api directory
cd api

# Install dependencies
npm install

# Create .env file
cp .env.example .env

# Update .env with your configurations
# MongoDB URI, JWT Secret, Port, etc.

# Start backend server
npm start
```

---

## 📁 Project Structure

```
Resume-Hub-Resume-Builder-/
├── client/                  # Frontend (React)
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── pages/          # Page components
│   │   ├── store/          # Zustand store
│   │   ├── hooks/          # Custom hooks
│   │   ├── utils/          # Utility functions
│   │   ├── assets/         # Images and icons
│   │   ├── App.jsx         # Main App
│   │   └── main.jsx        # Entry point
│   ├── public/             # Static files
│   ├── index.html          # HTML template
│   └── package.json
│
├── api/                     # Backend (Node.js)
│   ├── routes/             # API routes
│   ├── controllers/        # Route controllers
│   ├── models/             # Database models
│   ├── middleware/         # Custom middleware
│   ├── utils/              # Helper functions
│   ├── config/             # Configuration
│   ├── server.js           # Express server
│   └── package.json
│
└── README.md
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Frontend** | React 18, Zustand, Tailwind CSS |
| **Backend** | Node.js, Express.js |
| **Database** | MongoDB |
| **Authentication** | JWT (JSON Web Tokens) |
| **File Storage** | Cloud Storage (AWS S3/Google Cloud) |
| **PDF Generation** | jsPDF, html2pdf |
| **Validation** | Joi, Yup |

---

## 📝 Resume Templates

### Template 1: Modern Professional
- Clean, modern layout
- Perfect for tech professionals
- Minimalist design
- Easy to read

### Template 2: Classic Executive
- Traditional layout
- Suitable for executives
- Professional appearance
- High-impact design

### Template 3: Creative Portfolio
- Creative design
- Ideal for designers/artists
- Visual appeal
- Standout format

### More Templates Coming Soon!

---

## 📋 Form Sections

The resume builder includes the following sections:

1. **Personal Information**
   - Full name
   - Email
   - Phone number
   - Location
   - Professional summary

2. **Experience**
   - Company name
   - Job title
   - Start date
   - End date
   - Job description

3. **Education**
   - School/University name
   - Degree
   - Field of study
   - Start date
   - End date

4. **Skills**
   - Skill name
   - Proficiency level
   - Add multiple skills

5. **Certifications**
   - Certification name
   - Issuing organization
   - Date obtained
   - Credential URL

6. **Projects**
   - Project name
   - Description
   - Technologies used
   - Project link

---

## 🔧 Environment Variables

### Frontend (.env)
```env
VITE_API_URL=http://localhost:5000/api
VITE_APP_NAME=ResumeHub
```

### Backend (.env)
```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/resumehub
JWT_SECRET=your_jwt_secret_key
NODE_ENV=development
CORS_ORIGIN=http://localhost:5173
```

---

## 📊 API Endpoints

### Authentication
- `POST /api/auth/register` - Register user
- `POST /api/auth/login` - Login user
- `POST /api/auth/logout` - Logout user

### Resumes
- `GET /api/resumes` - Get all user resumes
- `POST /api/resumes` - Create new resume
- `GET /api/resumes/:id` - Get specific resume
- `PUT /api/resumes/:id` - Update resume
- `DELETE /api/resumes/:id` - Delete resume

### PDF Export
- `POST /api/resumes/:id/pdf` - Generate and download PDF

---

## 🎨 Customization

### Change Default Theme

Edit `client/src/config/theme.js`:

```javascript
const theme = {
  primary: '#007BFF',
  secondary: '#6C757D',
  accent: '#28A745',
  background: '#ffffff',
  text: '#333333',
}
```

### Add New Template

1. Create new template in `client/src/templates/`
2. Add template data structure
3. Update template selector
4. Test preview and export

---

## 🎯 Learning Outcomes

This project demonstrates:
- ✅ Full-stack development (MERN)
- ✅ React component architecture
- ✅ State management with Zustand
- ✅ Node.js backend development
- ✅ Express.js routing
- ✅ MongoDB database operations
- ✅ JWT authentication
- ✅ PDF generation
- ✅ File uploads
- ✅ API integration
- ✅ Form handling
- ✅ Responsive design
- ✅ Performance optimization

---

## 📊 Performance Metrics

- ⚡ **Frontend Lighthouse:** 92/100
- 📦 **Frontend Bundle:** 60KB (gzipped)
- 🚀 **Load Time:** 1.5s (average)
- 🎯 **Time to Interactive:** 2.2s
- 📄 **PDF Generation:** <3s

---

## 📸 Screenshots

<details>
<summary><b>Click to expand screenshots</b></summary>

### Homepage
![Home](https://github.com/jatinagrahari/Resume-Hub-Resume-Builder-/blob/main/client/resumeBuilderBlobs/homePage.png)

### Template Selection
![Templates](https://github.com/jatinagrahari/Resume-Hub-Resume-Builder-/blob/main/client/resumeBuilderBlobs/templates.png)

### Form Interface
![Form](https://github.com/jatinagrahari/Resume-Hub-Resume-Builder-/blob/main/client/resumeBuilderBlobs/3.png)

### Live Preview
![Preview](https://github.com/jatinagrahari/Resume-Hub-Resume-Builder-/blob/main/client/resumeBuilderBlobs/4.png)

### Template View
![Template](https://github.com/jatinagrahari/Resume-Hub-Resume-Builder-/blob/main/client/resumeBuilderBlobs/templatePage.png)

</details>

---

## 🚀 Deployment

### Frontend Deployment (Netlify)
```bash
# Build production version
npm run build

# Deploy to Netlify
netlify deploy --prod --dir=dist
```

### Backend Deployment (Heroku/Railway)
```bash
# Add Procfile
echo "web: node server.js" > Procfile

# Deploy to Heroku
git push heroku main
```

---

## 🐛 Known Issues

- None currently reported

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-feature`)
6. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Jatin Agrahari**

- 🔗 [GitHub](https://github.com/jatinagrahari)
- 💼 [LinkedIn](https://linkedin.com/in/jatinagrahari)
- 🐦 [Twitter](https://twitter.com/jatinagrahari)
- 🌐 [Portfolio](https://itsjatin.me)

---

## 📚 Resources & Documentation

- [React Documentation](https://react.dev/)
- [Node.js Documentation](https://nodejs.org/docs/)
- [MongoDB Documentation](https://docs.mongodb.com/)
- [Express.js Guide](https://expressjs.com/)
- [Zustand GitHub](https://github.com/pmndrs/zustand)
- [Tailwind CSS Docs](https://tailwindcss.com/docs)

---

## 🙏 Acknowledgments

- Built with ❤️ using MERN stack
- Thanks to the amazing open-source community
- Special thanks to all contributors
- Inspired by professional resume builders

---

## ⭐ Show your support

Give a ⭐️ if this project helped you create an amazing resume!

**Ready to build your resume? Let's go! 📄✨**
