# DevPilot 🚀
**AI-Powered GitHub Repository Assistant**
DevPilot is an AI-powered developer tool that helps developers understand and explore their codebases through conversational AI. Connect your GitHub repositories, index source code, and ask questions about your code using natural language.
## ✨ Features
- 🔐 GitHub OAuth 2.0 authentication
- 📂 GitHub repository integration
- 🔎 Automated source code indexing
- 🤖 AI-powered codebase chat
- 💬 Streaming chat responses
- 🧠 Context-aware code retrieval
- 📑 Code citations in AI responses
- 🗂️ Repository-specific chat sessions
- 🎨 Modern, responsive user interface
## 🛠️ Tech Stack
### Frontend
- Next.js
- React
- TypeScript
- Tailwind CSS
### Backend
- Java
- Spring Boot
- Spring Security
- Spring AI
- Maven
### Database and AI
- PostgreSQL
- pgvector
- Ollama
- GitHub OAuth 2.0
### Infrastructure
- Docker Compose
## 📁 Project Structure
```text
devPilot/
├── backend/
│   ├── src/
│   ├── pom.xml
│   └── mvnw
├── client/
│   ├── app/
│   ├── components/
│   ├── hooks/
│   ├── lib/
│   └── package.json
├── docker/
│   └── postgres/
├── docker-compose.yml
└── README.md
````
## ⚙️ Prerequisites
Before running DevPilot, install:
* Java compatible with the backend configuration
* Node.js and npm
* Docker Desktop
* Git
* GitHub OAuth application credentials
* Ollama and the required AI models
## 🚀 Getting Started
### 1. Clone the repository
```bash
git clone https://github.com/shivam123450/devPilot.git
cd devPilot
```
### 2. Configure the backend
Create a local configuration file from the example:
**Windows PowerShell:**
```powershell
Copy-Item backend/src/main/resources/application.example.properties backend/src/main/resources/application.properties
```
Configure the required database credentials, GitHub OAuth credentials, encryption settings, and application URLs.
Use environment variables or local configuration for sensitive values. Never commit passwords, OAuth secrets, or private encryption keys.
### 3. Start PostgreSQL
If the PostgreSQL service is defined in Docker Compose, run:
```bash
docker compose up -d postgres
```
Ensure PostgreSQL and the pgvector extension are ready before starting the backend.
### 4. Start the backend
From the project root:
```powershell
cd backend
.\mvnw.cmd spring-boot:run
```
The backend is configured to use port `8080` by default.
### 5. Start the frontend
Open another terminal at the project root:
```powershell
cd client
npm install
npm run dev
```
Open the application at:
http://localhost:3000
> Complete the required configuration before running the application. GitHub authentication and AI features require their respective services and credentials.
## 🔒 Security
* Keep credentials in environment variables or local configuration files.
* Never commit OAuth secrets, passwords, or private keys.
* Configure OAuth callback URLs correctly.
* Use appropriate CORS settings for your deployment environment.
## 🗺️ Roadmap
* [ ] Complete local setup documentation
* [ ] Expand automated test coverage
* [ ] Deploy the application
* [ ] Add screenshots and a live demo
* [ ] Improve monitoring and error handling
## 👨‍💻 Author
**Shivam Vishwakarma**
GitHub: [@shivam123450](https://github.com/shivam123450)
---
⭐ If you find this project interesting, consider starring the repository.
