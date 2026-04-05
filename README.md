<div align="center">
  
  # 💸 FinFlow: Your Personal FinAI & Smart Expense Tracker

  **An intelligent, real-time expense management and splitting platform powered by Generative AI.**

  [![Live Demo](https://img.shields.io/badge/Live_Demo-View_Project-2ea44f?style=for-the-badge&logo=vercel)](https://coincious-smart-expense.vercel.app/)
  
  <p align="center">
    <a href="https://react.dev/"><img src="https://img.shields.io/badge/React_18-20232A?style=flat&logo=react&logoColor=61DAFB" alt="React" /></a>
    <a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/TypeScript-007ACC?style=flat&logo=typescript&logoColor=white" alt="TypeScript" /></a>
    <a href="https://flask.palletsprojects.com/"><img src="https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white" alt="Flask" /></a>
    <a href="https://python.org"><img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python" /></a>
    <a href="https://supabase.com/"><img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat&logo=supabase&logoColor=white" alt="Supabase" /></a>
    <a href="https://tailwindcss.com/"><img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white" alt="Tailwind" /></a>
    <a href="https://ai.google/dev/"><img src="https://img.shields.io/badge/Google_Gemini-8E75B2?style=flat&logo=google-bard&logoColor=white" alt="Gemini AI" /></a>
  </p>

  *Streamline your finances, split bills effortlessly with friends, and let AI analyze your spending habits.*

</div>

---

## 📖 Project Overview

**FinFlow** is a modern, full-stack web application designed to solve the complexities of personal finance and group expense splitting. Built with a React/TypeScript frontend and a Python/Flask backend, it leverages **Generative AI (Google Gemini & Groq)** to automatically categorize expenses and provide an interactive financial chatbot. 

Backed by **Supabase** for secure authentication and real-time database synchronization, FinFlow offers a seamless, collaborative experience across devices.

### Why this project stands out:
- **AI Integration:** Moves beyond basic CRUD operations by implementing LLMs for intelligent data categorization and interactive user support.
- **Real-Time Collaboration:** Uses Supabase's real-time subscriptions for instant updates across group members.
- **Robust Architecture:** Clean separation of concerns between a highly interactive React frontend and a scalable Python REST API.

---

## ✨ Key Features

- **🤖 AI-Powered Categorization:** Automatically classifies spending and receipts using Google Generative AI, removing manual data entry.
- **💬 Smart Financial Chatbot:** Built-in AI assistant to provide personalized financial insights and answer expense-related queries.
- **👥 Advanced Group Management:** Create groups, track shared expenses, and calculate optimal settlement routes (who owes whom).
- **📊 Visual Analytics:** Interactive charts and graphs (via Recharts) to visualize spending trends over time.
- **🔐 Secure & Real-Time:** Full JWT-based user authentication and real-time data syncing powered by Supabase.
- **👨‍👩‍👧‍👦 Parental Controls:** Monitor family expenses and set smart spending limits.
- **🌗 Modern UI/UX:** Fully responsive design with Dark Mode, built using Tailwind CSS, Radix UI, and Framer Motion.

---

## 🛠️ Tech Stack

### **Frontend**
* **Framework:** React 18, Vite
* **Language:** TypeScript
* **Styling:** Tailwind CSS, Radix UI (Headless components)
* **Animations:** Framer Motion (`motion`)
* **Data Visualization:** Recharts
* **State/Forms:** React Hook Form, React Context API

### **Backend**
* **Framework:** Python 3.10+, Flask
* **AI/LLM:** Google Generative AI API, Groq API
* **Server:** Gunicorn (for production)
* **Image Processing:** Pillow (for receipt scanning/handling)

### **Database & Infrastructure**
* **BaaS:** Supabase (PostgreSQL, Auth, Real-time Subscriptions)
* **Hosting:** Vercel (Frontend) / Render (Backend)

---

## 🚀 Getting Started (Local Development)

To get a local copy up and running, follow these simple steps.

### Prerequisites
* **Node.js** (v18 or higher)
* **Python** (v3.10 or higher)
* **Supabase Account** (Create a free project at [supabase.com](https://supabase.com))
* **Google Gemini API Key**

### 1. Clone the Repository
```bash
git clone [https://github.com/YOUR_GITHUB_USERNAME/FinFlow.git](https://github.com/YOUR_GITHUB_USERNAME/FinFlow.git)
cd FinFlow
```

### 2. Backend Setup (Flask API)
Open a terminal and navigate to the backend directory:

```bash
cd backend
```

# Create and activate a virtual environment

```bash
python -m venv venv
source venv/bin/activate      # On Windows use: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Environment Setup
touch .env
```
Add the following to your backend .env file:

```bash
GEMINI_API_KEY=your_gemini_api_key_here
GROQ_API_KEY=your_groq_api_key_here
```
Run the backend server:

```bash
python run.py
# The Flask API will start on http://localhost:8000
```
### 3. Frontend Setup (React/Vite)
Open a new terminal and navigate to the frontend directory:

```bash
cd Frontend

# Install dependencies
npm install

# Environment Setup
cp .env.example .env.local
```
Add your Supabase credentials to .env.local:

```
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```
Start the frontend development server:

```bash
npm run dev
# The application will open at http://localhost:3000
```
📡 API Reference (Backend)
The backend provides RESTful endpoints to interact with the AI models.

Categorize Expense via AI
$POST /api/categorize$

Body:

```JSON
{
  "description": "Uber ride to the airport",
  "amount": 45.50
}
```
Returns: AI-determined category (e.g., Travel) based on context and historical data.

🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page.
- Fork the Project
- Create your Feature Branch (git checkout -b feature/AmazingFeature)
- Commit your Changes (git commit -m 'Add some AmazingFeature')
- Push to the Branch (git push origin feature/AmazingFeature)
- Open a Pull Request


<div align="center">
<b>Built by <a href="https://www.google.com/search?q=https://github.com/Tirthgandhi05">Tirth Gandhi</a></b>


<i>If you like this project, please leave a ⭐!</i>
</div>
