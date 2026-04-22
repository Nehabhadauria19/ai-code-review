# 🚀 AI Code Review Platform

An AI-powered full-stack application that analyzes source code for **bugs, security vulnerabilities, performance issues, and best practices** using LLMs.

---

## 🌟 Features

* 🔍 **Automated Code Analysis**
  Detects bugs, security risks, and performance bottlenecks.

* 🧠 **AI-Powered Reviews**
  Uses Groq LLM to generate structured, developer-friendly feedback.

* 📊 **Severity Classification**
  Categorizes issues into low, medium, and high severity.

* 🧾 **Review History**
  Stores past reviews with timestamps using MongoDB.

* ⚡ **Fallback Mechanism**
  Ensures reliable output even when AI responses are incomplete.

* 🎨 **Modern UI**
  Clean and responsive interface built with Next.js.

---

## 🛠️ Tech Stack

### Frontend

* Next.js
* React
* Tailwind CSS

### Backend

* Node.js
* Express.js

### Database

* MongoDB

### AI Integration

* Groq API (LLM)

---

## 📂 Project Structure

```
ai-code-review/
│
├── backend/
│   ├── routes/
│   ├── services/
│   ├── models/
│   ├── config/
│   └── server.js
│
├── frontend/
│   ├── app/
│   ├── components/
│   └── lib/
│
└── README.md
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the repository

```
git clone https://github.com/YOUR_USERNAME/ai-code-review.git
cd ai-code-review
```

---

### 2️⃣ Setup Backend

```
cd backend
npm install
```

Create a `.env` file:

```
PORT=5000
MONGO_URI=your_mongodb_uri
GROQ_API_KEY=your_groq_api_key
GROQ_MODEL=llama-3.1-8b-instant
```

Run backend:

```
npm run dev
```

---

### 3️⃣ Setup Frontend

```
cd frontend
npm install
npm run dev
```

---

## 🔗 API Endpoints

### Analyze Code

```
POST /api/review
```

**Body:**

```
{
  "code": "your code here",
  "language": "javascript"
}
```

---

### Get Review History

```
GET /api/reviews
```

---

## 🧪 Example

### Input

```js
function test() {
  var x = 10;
}
```

### Output

```
Best Practices:
- Avoid using 'var', use 'let' or 'const'
```

---

## 🚀 Deployment

* Frontend: Vercel
* Backend: Render

---

## 📌 Future Improvements

* Line-by-line code suggestions
* Multi-language support
* GitHub PR integration
* Real-time collaboration

---

## 👩‍💻 Author

**Neha Bhadauria**

* GitHub:https://github.com/Nehabhadauria19/ai-code-review

---

## ⭐ Support

If you like this project, consider giving it a ⭐ on GitHub!
