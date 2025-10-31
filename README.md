🧭 Job-Pilot

Job-Pilot is a full-stack web application designed to connect job seekers and recruiters in a single platform.
It provides an AI-powered job hiring system where candidates can apply for jobs, give coding and aptitude tests, and appear for interviews — while recruiters can manage applications, conduct interviews, and evaluate performance.

🚀 Features
👨‍💼 For Job Seekers:

Create a professional profile and upload resumes.

Attempt aptitude and coding tests.

Attend live interview sessions with screen-sharing support.

Track application progress and results.

🏢 For Recruiters / Companies:

Post job openings with required skills and test details.

Review candidate profiles, test results, and interview feedback.

Conduct interviews directly through the platform.

Manage and track candidates efficiently.

🔒 Authentication:

Secure login using Supabase Auth with Email-Password and LinkedIn OAuth.

💬 Interview System:

Interviewer can view candidate’s screen and code in real time.

Built-in code editor and chat for interaction.

🧠 AI Assistance:

Integrated AI helper to generate coding questions and analyze responses.

🛠️ Tech Stack
Layer	Technology
Frontend	React.js, Vite, Tailwind CSS
Backend	Node.js, Express.js
Database	Supabase (PostgreSQL)
Authentication	Supabase Auth (Email + LinkedIn OAuth)
Cloud Storage	Supabase Storage
Realtime Communication	WebRTC / Socket.io
AI Integration	OpenAI / Gemini API (for question generation & evaluation)
📂 Project Structure
Job-Pilot/
├── frontend/                     # React.js Frontend
│   ├── src/                      # Main source code (components, pages, hooks)
│   │   ├── components/           # UI Components (Navbar, Dashboard, etc.)
│   │   ├── pages/                # App Pages (Login, Register, Test, Interview)
│   │   ├── context/              # Global Context (Auth, Test, Interview)
│   │   ├── utils/                # Helper functions (API calls, constants)
│   │   └── App.jsx               # Root Component
│   ├── public/                   # Static assets (icons, logos, index.html)
│   └── package.json              # Frontend dependencies and scripts
│
├── backend/                      # Node.js Backend
│   ├── controllers/              # API Controllers (business logic)
│   ├── models/                   # MongoDB Models (schemas)
│   ├── routes/                   # Express Routes (API endpoints)
│   ├── middleware/               # Authentication & authorization middleware
│   ├── utils/                    # Helper functions (AI utils, resume parser)
│   ├── config/                   # Database & cloud configuration
│   └── server.js                 # Main server entry point
│
├── .env                          # Environment variables (API keys, DB URLs)
└── README.md                     # Project documentation

⚙️ Installation & Setup
1️⃣ Clone the repository:
git clone https://github.com/THE-DEEPDAS/Medhavi-Full.git
cd Job-Pilot

2️⃣ Setup Frontend:
cd frontend
npm install
npm run dev

3️⃣ Setup Backend:
cd backend
npm install
npm run dev

4️⃣ Configure Environment Variables:

Create a .env file in the backend folder and add:

PORT=5100
SUPABASE_URL=your_supabase_project_url
SUPABASE_KEY=your_supabase_api_key
JWT_SECRET=your_secret_key
OPENAI_API_KEY=your_openai_key

🧩 Workflow

User signs up or logs in using Supabase Auth.

Job seeker completes profile and starts aptitude or coding tests.

Recruiter posts jobs and reviews applicants’ performance.

Interview round conducted with integrated screen-sharing and live code editor.

Recruiter finalizes candidate and updates job status.
