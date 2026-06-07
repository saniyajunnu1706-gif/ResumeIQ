# 🧠 Resume IQ — AI-Powered Resume Screening Tool

A live AI-powered recruitment tool that automatically screens, scores, and shortlists candidates from multiple resumes using Anthropic Claude AI.

---

## 🔗 Live Demo

https://resumeiq-1706.netlify.app

Email: resumeiq@company.com
Password: demo1234

---

## 📌 Problem Statement

Recruiters receive hundreds of resumes for a single job posting and spend 5 to 8 hours reading them manually. This process is slow, biased and inconsistent. Resume IQ solves this by using Generative AI to automatically screen all resumes in minutes and give objective scores and recommendations.

---

## ✨ Features

- Authentication System — Login, Signup, Forgot Password, Google OAuth, Microsoft OAuth
- Multi Resume Upload — Drag and drop multiple PDF, DOC, DOCX, TXT files at once
- AI Resume Scoring — Claude AI scores each resume against the job description
- 4 Dimension Scoring — Skills, Experience, Education and Overall out of 100
- Smart Recommendations — Shortlist, Maybe or Reject for each candidate
- Strict Field Matching — Rejects candidates from completely wrong fields
- Demo Mode — Works without API key for showcasing
- Real AI Mode — Full Claude AI analysis with API key
- Filter and Compare — Filter by recommendation, compare up to 4 candidates
- CSV Export — Export all results or selected candidates
- Account Settings — Edit profile, manage API key, billing plans, team members
- Billing Plans — Free, Pro and Enterprise with monthly and annual toggle

---

## 🛠️ Tech Stack

HTML5 — Structure and layout
CSS3 — Styling and animations
Vanilla JavaScript — Logic and state management
Anthropic Claude API — AI resume analysis
REST API fetch — API communication
FileReader API — Resume text extraction
Netlify — Deployment and hosting

---

## 🤖 How AI Scoring Works

1. Recruiter pastes the Job Description
2. Recruiter uploads multiple resumes
3. App extracts text from each resume using FileReader API
4. Text is sent to Claude AI with a structured prompt
5. Claude returns JSON with scores and recommendation
6. Results displayed as visual cards with score bars

Scoring Rules:
- 85 to 100 — Excellent match — Shortlist
- 70 to 84 — Good match — Shortlist
- 50 to 69 — Partial match — Maybe
- 30 to 49 — Poor match — Reject
- 0 to 29 — No match or Wrong field — Reject

Strict Rejection Rules:
- Skills score below 40 — Always Reject
- Experience score below 35 — Always Reject
- Overall score below 50 — Always Reject
- Completely wrong field — Skills 0 to 15 — Always Reject

---

## ⚡ Demo Mode vs Real AI Mode

Demo Mode:
- No API key required
- Free — zero cost
- Name extracted from real resume
- Field mismatch detection works
- Scores are simulated

Real AI Mode:
- API key required
- Cost is approximately $0.01 per resume
- Name extracted from real resume
- Field mismatch detection works
- Scores are real Claude AI analysis

---

## 🚀 Getting Started

Option 1 — Use Live Site
Visit https://resumeiq-1706.netlify.app and login with demo credentials

---

## 🔑 API Key Setup For Real AI Mode

1. Go to console.anthropic.com
2. Sign up and get free credits
3. Create an API key
4. In the app click avatar then API Key Settings
5. Paste your key and save
6. Demo banner disappears and real AI mode is active

---

## 💡 Prompt Engineering

The AI prompt is carefully designed to:
- Tell Claude to act as an expert recruiter
- Inject job description and resume text dynamically
- Return strict JSON format with exact keys
- Enforce field mismatch detection
- Restrict recommendation to exactly 3 values — Shortlist Maybe Reject
- Override lenient AI responses with strict score enforcement

---

## 🔮 Future Improvements

- Backend proxy to hide API key securely
- PDF text extraction using pdf.js
- Database to save candidate history
- ATS integration with Greenhouse and Lever
- Bulk email to shortlisted candidates
- Analytics dashboard for hiring metrics
- Pro subscription with payment gateway

---

## 📊 Business Impact

Manual Screening — 50 resumes — 5 to 8 hours — recruiter salary cost
Resume IQ — 50 resumes — 5 to 10 minutes — less than $1 cost
Consistency — manual varies — Resume IQ always consistent
Bias — manual has human bias — Resume IQ gives objective scoring

---

## 🏗️ Project Structure

resume-iq/
├── index.html     — Complete single file application with HTML CSS and JavaScript
└── README.md      — Project documentation

---

## 👩‍💻 About the Developer

Saniya Firdous
Generative AI Engineer — LLM Integration — Prompt Engineering — RAG Systems

Email: saniyajunnu1706@gmail.com
Location: Palamaner, Chittoor, India

---

## 🙏 Acknowledgements

- Anthropic for the Claude AI API
- Netlify for free hosting
- Google Fonts for DM Sans and Playfair Display

---

If you found this project helpful please give it a star!
