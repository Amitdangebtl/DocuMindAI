# 🚀 DocuMindAI

AI-powered **Document Intelligence System** built using:

- **ASP.NET Core MVC** (Frontend UI)
- **ASP.NET Core Web API** (Backend)
- **MongoDB** (Database)
- **OpenAI** (AI Processing)
- **Qdrant** (Vector Database)

This system allows users to upload documents and ask AI questions based on document content.

---

# 📌 Project Overview

DocuMindAI is a **full-stack AI-powered document processing platform** where users can:

- 📄 Upload documents
- 🗄 Store document metadata in MongoDB
- 🧠 Generate embeddings using OpenAI
- 📊 Store embeddings in Qdrant Vector Database
- ❓ Ask AI questions based on uploaded documents
- 🔐 Secure APIs using JWT + HMAC
- 💳 Control access using subscription logic

---

# 🏗️ Solution Architecture

The solution contains **two main projects**

---

## 1️⃣ MVCSimpleUplode (Frontend - MVC)

Responsible for:

- Razor UI Pages
- Login & Register
- Admin Dashboard
- Document Upload UI
- Ask AI Interface
- API Integration using HttpClient

### Structure

```
Controllers/
Views/
Models/
wwwroot/
```

---

## 2️⃣ SimpleUplode (Backend - Web API)

Responsible for:

- REST API endpoints
- Business logic
- MongoDB database operations
- OpenAI integration
- Qdrant vector storage
- Security middleware
- Subscription validation

### Structure

```
Controllers/
Models/
Services/
Filters/
Security/
```

### Important Components

- AiController  
- DocumentController  
- AuthController  
- QdrantController  
- SubscriptionFilter  
- HmacMiddleware  
- OpenAIService  
- QdrantService  
- MongoServices  

---

# 🔐 Security Features

✔ JWT Authentication  
✔ HMAC Request Signature Validation  
✔ Subscription Based Access Control  
✔ Middleware Request Protection  

---

# 🛠️ Technologies Used

- ASP.NET Core MVC
- ASP.NET Core Web API
- C#
- MongoDB
- OpenAI API
- Qdrant Vector Database
- JWT Authentication
- Docker
- Swagger

---

# ⚙️ How to Run

## 1️⃣ Configure MongoDB

Update **appsettings.json**

```json
"MongoDbSettings": {
  "ConnectionString": "mongodb://localhost:27017",
  "DatabaseName": "DocuMindAI"
}
```

---

## 2️⃣ Run Backend API

```
dotnet run --project SimpleUplode
```

---

## 3️⃣ Run MVC Frontend

```
dotnet run --project MVCSimpleUplode
```

---

# 🐳 Run With Docker

```
docker-compose up --build
```

---

# 📌 Major API Endpoints

### Upload Document

```
POST /api/document/upload
```

### Ask AI

```
POST /api/ai/ask
```

Example Request

```json
{
  "question": "Explain .NET Developer role",
  "documentId": "document-id"
}
```

---

# 📷 Application Screenshots

## 🔹 Login Page
![Login](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/LoginPage.png)

---

## 🔹 Register Page
![Register](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/RegisterPage.png)

---

## 🔹 Home Page
![HomePage](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/HomePage(1).png)

---

## 🔹 Home Page (Alternate)
![HomePage2](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/Home%20Page(2).png)

---

## 🔹 User Dashboard
![UserDashboard](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/User%20Deshboard.png)

---

## 🔹 Admin Dashboard
![AdminDashboard](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/Admin%20Deshboard.png)

---

## 🔹 Upload Document
![UploadDocument](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/Upload%20Document.png)

---

## 🔹 My Documents
![MyDocuments](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/My%20Documents.png)

---

## 🔹 My Profile
![MyProfile](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/My%20Profile.png)

---

## 🔹 Ask AI
![AskAI](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/Ask%20AI.png)

---

## 🔹 Admin Manage Documents
![AdminManageDocs](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/Admin%20Manage%20All%20Documents.png)

---

## 🔹 Admin Users Management
![AdminUsers](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/Admin%20Users%20Management.png)

---

## 🔹 Swagger API (1)
![Swagger1](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/Swagger%20API%20(1).png)

---

## 🔹 Swagger API (2)
![Swagger2](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/Swagger%20API%20(2).png)

---

## 🔹 Docker Containers
![Docker](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/Docker%20Containers.png)

---

## 🔹 Qdrant Vector Database
![Qdrant](https://raw.githubusercontent.com/Amitdangebtl/DocuMindAI/main/Qdrant.png)

---

# 🎯 Key Highlights

✔ Full Stack AI Application  
✔ Document-based AI Q&A System  
✔ Vector Search using Qdrant  
✔ Secure API Architecture  
✔ MongoDB NoSQL Integration  
✔ Dockerized Deployment  

---

# 👨‍💻 Author

**Amit Dange**

.NET Developer  
ASP.NET Core | AI Integration | MongoDB
