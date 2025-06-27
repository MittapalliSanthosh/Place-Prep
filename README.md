# PlacePrep - Placement Preparation Platform

A full-stack web application to help engineering students prepare for campus placements with mock tests, interview practice, AI explanations, and more.

## 🚀 Features

- **Multi-Department Support:** CSE, ECE, EEE, Civil, Mechanical, Chemical Engineering
- **Mock Tests:** Practice assessments with real-time scoring, AI explanations, and progress tracking
- **Interview Preparation:** Comprehensive interview question bank and tips, AI-powered mock interviews
- **Aptitude Tests:** Quantitative, logical, and verbal reasoning practice
- **Notes Management:** Personal note-taking and sharing system
- **Progress Tracking:** Monitor learning progress across different modules
- **User Authentication:** Secure login with Google OAuth integration
- **AI Integration:** Google Gemini API for explanations and interview feedback

## 🛠️ Tech Stack

**Frontend:**  
- HTML5, CSS3, JavaScript (ES6+), Bootstrap

**Backend:**  
- Node.js, Express.js, MongoDB (Mongoose)
- (Optional) Firebase for authentication only

**AI:**  
- Google Gemini API

---

## 📁 Project Structure

```
Place-Prep/
├── server.js
├── package.json
├── .gitignore
├── README.md
├── .env (not committed)
├── serviceAccountKey.json (not committed)
├── models/
│   ├── Question.js
│   ├── MockTestProgress.js
│   ├── InterviewFeedback.js
│   └── Note.js
├── utils/
│   └── emailService.js
├── HTML/
│   ├── landingpage.html
│   ├── login.html
│   ├── signup.html
│   ├── placement_website.html
│   ├── mocktest.html
│   ├── module.html
│   ├── interview.html
│   ├── notes.html
│   ├── profile.html
│   ├── shownotes.html
│   ├── code.html
│   ├── Civil_department.html
│   ├── cse_department.html
│   ├── ece_department.html
│   ├── mechanical_department.html
│   ├── chemical.html
│   ├── electrical.html
│   ├── aptitude.html
│   ├── 404.html
│   └── js/
│       ├── aptitude_data.js
│       ├── chemical_data.js
│       ├── civil_data.js
│       ├── cse_data.js
│       ├── ece_data.js
│       ├── electrical_data.js
│       ├── interview_data.js
│       ├── mechanical_data.js
│       ├── mocktest_data.js
│       └── notes_data.js
├── importQuestions.js
├── seedAssessments.js
├── checkDatabase.js
├── resetDatabase.js
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm (v6 or higher)
- MongoDB Atlas or local MongoDB
- Google Cloud account (for Gemini API)
- (Optional) Firebase for authentication

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/MittapalliSanthosh/Place-Prep.git
   cd Place-Prep
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Configuration**
   - Create a `.env` file in the root directory:
     ```
     GEMINI_API_KEY=your-google-gemini-api-key
     MONGODB_URI=your-mongodb-uri
     GOOGLE_CLIENT_ID=your-google-client-id
     ```
   - Do **not** commit `.env` to GitHub.

4. **Database Setup**
   ```bash
   node importQuestions.js
   node seedAssessments.js
   ```

5. **Start the server**
   ```bash
   npm start
   # or
   node server.js
   ```

6. **Access the application**
   - Open `http://localhost:3000` in your browser

---

## 🌐 Deployment (Render)

1. Push your code to GitHub.
2. Create a new Web Service on [Render](https://render.com/).
3. Connect your GitHub repo.
4. Set environment variables (`GEMINI_API_KEY`, `MONGODB_URI`, etc.) in the Render dashboard.
5. Deploy!

---

## 📖 Usage Guide

- Register/Login (Google OAuth supported)
- Select your department
- Take mock tests, view explanations, and track your progress
- Use the AI Interviewer for practice and feedback

---

## 🐛 Troubleshooting

- **500 Internal Server Error:** Check your API key, quota, and environment variables.
- **MongoDB errors:** Ensure your `MONGODB_URI` is correct and accessible.
- **Gemini API quota exceeded:** Wait for quota reset or upgrade your Google Cloud plan.

---

## 👥 Author

- **Mittapalli Santhosh Kumar**

---

## 📄 License

This project is licensed under the MIT License.

---

**For academic use only. For support, create an issue or contact: santhoshkumarmittapalli7@gmail.com**
