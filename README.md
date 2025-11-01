💸 FinSphere — AI-Powered Financial Inclusion Platform
🧠 DATATHON 2K25 — Final Round Submission

Theme: AI-Powered Financial Inclusion & Intelligent Credit Ecosystem for the Next Billion Users

🌍 Overview

FinSphere is an end-to-end AI-powered fintech platform designed to promote financial inclusion for freelancers, students, farmers, and gig workers who are often excluded by traditional banking systems.

It uses alternative data, AI/ML models, and explainable insights to build trust, offer fair credit access, and empower financial literacy for the next billion users.

⚙️ Core Modules
1️⃣ Alternative Credit Scoring Engine

Uses non-traditional data (UPI patterns, spending behavior, mobile usage) to estimate creditworthiness.

Integrates pretrained models (DistilBERT, BERT-base-uncased) fine-tuned on:

Financial PhraseBank

Credit Risk Dataset (Kaggle)

Provides Explainable AI (XAI) output — “Why this person got this score?”

2️⃣ Smart Personal Finance Dashboard

Tracks income, expenses, and savings

Generates AI-driven insights and dynamic “Financial Health Index”

Shows graphs, recommendations, and personalized advice

Allows users to input:

Mood/stress levels

Spending habits

Savings goals
→ Updates insights dynamically

3️⃣ AI Financial Mentor / Chatbot

Acts as a personal finance guide in local languages

Explains loans, EMIs, and investment options

Lightweight design supports offline/rural use cases

4️⃣ Fraud Detection & Risk Intelligence

Detects fake KYCs, money laundering, or suspicious spending

Optionally integrates OpenAI or Gemini API for text-based fraud detection (“Is this SMS or message fraudulent?”)

Displays real-time static alerts or anomaly cards in dashboard

5️⃣ SaaS API Layer (Open Banking)

Your platform also acts as a service layer (API) that banks or NBFCs can plug into:

🔗 Endpoint:
https://hywuddqzrlcvbxvurpoh.supabase.co/functions/v1/finance-insights

🧩 Example Request (Test in Console or ReqBin):
fetch('https://hywuddqzrlcvbxvurpoh.supabase.co/functions/v1/finance-insights', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({ userId: 'demo-user-123' })
})
.then(r => r.json())
.then(data => console.log(data))

✅ Example Response:
{
  "user_id": "demo-user-123",
  "risk_score": 0.86,
  "financial_wellness_summary": "Strong credit behavior detected",
  "analysis": {
    "spending_trend": "stable",
    "savings_rate": "healthy",
    "credit_utilization": "optimal",
    "bill_payment_history": "excellent"
  },
  "recommendations": [
    "Continue maintaining current spending patterns",
    "Consider increasing emergency fund by 10%",
    "Optimize credit card usage for better rewards"
  ]
}


This proves real-world scalability and B2B potential for integration.

6️⃣ Financial Literacy Gamification

10–12 question interactive finance quiz 🧠

Points, badges & leaderboards for engagement

Responses stored locally (JSON/localStorage)

Boosts user education and retention

🧰 Tech Stack
Layer	Tools & Frameworks
Frontend	React + Tailwind CSS
Backend	Python (FastAPI)
AI Models	Hugging Face Transformers (DistilBERT/BERT-base-uncased)
Data Storage	JSON / localStorage (mock), Supabase (SaaS API)
Security	Secure local storage, mock data encryption
APIs	Open Banking API, SaaS /finance-insights, OpenAI/Gemini (fraud detection)


🧩 Project Highlights

Explainable AI Credit Scoring (XAI)

AI Chatbot Mentor (Multilingual)

SaaS API for Financial Insights

Fraud Detection via Text Classification

Dynamic Personal Finance Dashboard

Financial Literacy Gamification Zone

Mock Secure User Login/Signup

Local Data Encryption Simulation


🚀 Future Enhancements

Real-time UPI or SMS data ingestion

Blockchain-based KYC validation

Multilingual Voice Assistant

Carbon-neutral transaction tracking (FinTech + Sustainability)

DID (Decentralized Identity) integration

