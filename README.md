# ResumeGPT

An AI-powered resume generator built with React and Spring Boot that helps users create professional, ATS-friendly resumes with the assistance of artificial intelligence.

## 🚀 Features

- **AI-Powered Content Generation**: Leverage AI to generate professional resume content tailored to your experience
- **Real-time Preview**: See your resume updates in real-time as you enter information
- **ATS-Friendly Design**: Ensures your resume passes through Applicant Tracking Systems
- **Modern UI**: Clean, intuitive interface built with React
- **RESTful API**: Robust Spring Boot backend for handling resume generation logic
- **Export to PDF**: Download your completed resume as a professional PDF document

## 🛠️ Tech Stack

### Frontend
- **React** - UI library for building interactive user interfaces
- **JavaScript/TypeScript** - Programming language
- **CSS/Styled Components** - Styling and layout
- **Axios** - HTTP client for API communication

### Backend
- **Spring Boot** - Java framework for building the REST API
- **Spring Web** - For RESTful web services
- **Maven** - Dependency management
- **Ollama (Deepseek)** - AI integration for content generation

## 📋 Prerequisites

Before running this project, make sure you have the following installed:

- **Node.js** (v14 or higher)
- **npm** or **yarn**
- **Java JDK** (v11 or higher)
- **Maven** (v3.6 or higher)

## 🔧 Installation

### Clone the Repository

```bash
git clone https://github.com/VishalChavan7/ResumeGPT.git
cd ResumeGPT
```

### Backend Setup (Spring Boot)

1. Navigate to the backend directory:
```bash
cd backend
```

2. Configure your `application.properties`:
```properties
# Server Configuration
server.port=8080

# AI API Configuration (if using OpenAI or similar)
openai.api.key=your_api_key_here

# Database Configuration (if applicable)
spring.datasource.url=jdbc:mysql://localhost:3306/resumegpt
spring.datasource.username=your_username
spring.datasource.password=your_password
```

3. Install dependencies and run:
```bash
mvn clean install
mvn spring-boot:run
```

The backend server will start on `http://localhost:8080`

### Frontend Setup (React)

1. Navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
# or
yarn install
```

3. Create a `.env` file in the frontend directory:
```env
REACT_APP_API_URL=http://localhost:8080
```

4. Start the development server:
```bash
npm start
# or
yarn start
```

The frontend application will open at `http://localhost:3000`

## 📖 Usage

1. **Open the Application**: Navigate to `http://localhost:3000` in your browser
2. **Enter Your Information**: Fill in your personal details, work experience, education, and skills
3. **Generate with AI**: Use the AI assistance feature to enhance your resume content
4. **Preview**: Review your resume in real-time
5. **Download**: Export your resume as a PDF once you're satisfied

## 🏗️ Project Structure

```
ResumeGPT/
├── frontend/                 # React frontend application
│   ├── public/              # Static files
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── pages/          # Page components
│   │   ├── services/       # API service files
│   │   ├── utils/          # Utility functions
│   │   └── App.js          # Main App component
│   └── package.json
│
├── backend/                 # Spring Boot backend
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── com/resumegpt/
│   │   │   │       ├── controller/    # REST controllers
│   │   │   │       ├── service/       # Business logic
│   │   │   │       ├── model/         # Data models
│   │   │   │       ├── repository/    # Data access layer
│   │   │   │       └── config/        # Configuration files
│   │   │   └── resources/
│   │   │       └── application.properties
│   └── pom.xml
│
└── README.md
```

---

⭐ If you find this project helpful, please consider giving it a star on GitHub!
