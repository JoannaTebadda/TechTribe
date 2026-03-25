# PayTracka 

> **The mobile app that ends payment chaos for African freelancers**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-paytracka.lovable.app-0F6E56?style=for-the-badge)](https://paytracka.lovable.app)
[![Built With](https://img.shields.io/badge/Built%20With-React%20%2B%20Supabase-1652F0?style=for-the-badge)]()
[![AI Powered](https://img.shields.io/badge/AI%20Powered-Claude%20API-7C3AED?style=for-the-badge)]()
[![Payment](https://img.shields.io/badge/Payments-Interswitch%20API-E24B4A?style=for-the-badge)]()

---

## 🔗 Live Demo

**👉 [https://paytracka.lovable.app](https://paytracka.lovable.app)**

> Open in any browser on laptop or mobile. No installation required.

---

## 📌 Problem Statement

African freelancers receive income from 4 to 6 or more scattered platforms, Upwork, Fiverr, Payoneer, direct bank transfers. The average payment delay is **41 days** across Africa, **51 days in Nigeria** and **39 days in Kenya**. Freelancers waste **5 to 10+ hours every month** chasing late payments, have zero real-time visibility into their cash flow, and often dip into personal savings to cover income gaps.

**PayTracka solves this with one unified dashboard, a WhatsApp for your money.**

---

## 💡 Solution

PayTracka is a web-based payment tracking application that gives African freelancers:

- **One unified inbox** for all income from every platform
- **Who Owes Me tracker** — invoices sorted by urgency (overdue, due soon, paid)
- **One-tap smart reminders** — AI-generated WhatsApp/SMS messages sent instantly
- **Interswitch payment links** — clients pay directly from a link
- **AI-powered insights** — cash flow summaries, payment risk predictions, and income trends
- **Identity Verified badge** — BVN verification via Interswitch Identity API

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 🏠 Unified Dashboard | Real-time summary of total income, overdue, and pending amounts |
| 📥 Payment Inbox | All transactions from all platforms in one feed |
| 👤 Who Owes Me | Urgency-sorted Kanban — Overdue / Due Soon / Paid |
| 🔔 Smart Reminders | AI-generated reminder messages via WhatsApp or SMS |
| 🔗 Payment Links | Interswitch-powered payment links per invoice |
| 🤖 AI Cash Flow Summary | Natural language insight — "You are on track to earn ₦400k this month" |
| 📊 AI Payment Risk | Predicts which clients are likely to pay late |
| ✍️ AI Invoice Writer | Generates professional invoice descriptions automatically |
| 🛡️ BVN Verification | Identity verified badge via Interswitch Identity API |
| 💱 Multi-Currency | Toggle between ₦ NGN / KES / ZAR |
| ⏰ Smart Greeting | Time-based greeting based on user's local time |

---

## 🔌 Interswitch API Integration

PayTracka integrates with **3 Interswitch APIs**:

1. **Web Checkout API** — generates payment links clients use to pay invoices directly
2. **BVN Identity API** — verifies freelancer identity and displays the Identity Verified badge
3. **Transaction Search API** — powers the real-time insights and analytics dashboard

---

## 🤖 AI Integration

PayTracka uses the **Anthropic Claude API** for 4 intelligent features:

1. **AI Reminder Messages** — generates personalised, context-aware reminder messages based on client payment history
2. **AI Payment Risk Prediction** — analyses client behaviour and predicts delay risk (Low / Medium / High)
3. **AI Cash Flow Summary** — produces a plain-English summary of the freelancer's financial position
4. **AI Invoice Description Generator** — writes professional invoice descriptions from a simple service prompt

---

## 👥 Team & Contributions

> All team members — technical and non-technical — contributed to PayTracka. Below is a clear record of each person's involvement as required by the buildathon submission guidelines.

---

### 👩‍💼 Okoro Oluchi Ruth — Product Manager & Team Lead

**Role:** Product Manager, Researcher, Project Lead

**Contributions:**
- Led the entire product vision, strategy, and direction for PayTracka
- Conducted independent market research — sourced the 41-day payment delay statistic, identified the core pain points of African freelancers
- Developed the three user personas: Tolu (Nigerian graphic designer), Achieng (Kenyan web developer), and Kwame (Ghanaian writer)
- Wrote the full Product Requirements Document (PRD) including all Epics, User Stories, and Gherkin acceptance criteria
- Defined the MVP scope, feature prioritisation, and the 7-day sprint timeline
- Built the functional prototype using Lovable — designed all 7 screens, the colour system, and the UI/UX flow
- Managed the Supabase backend connection and environment variable configuration
- Coordinated team communication, tracked sprint progress, and managed the buildathon submission
- Prepared the demo script and pitch narrative

---

### 👩‍💼 Joanna Tebadda — Product Manager & UX Researcher

**Role:** Product Manager, User Experience, Quality Assurance

**Contributions:**
- Contributed to product requirements definition and feature scoping
- Reviewed and validated user stories and acceptance criteria against real freelancer pain points
- Conducted user experience review of all screens — provided feedback on usability, flow, and layout
- Assisted with quality assurance — tested all features including invoice creation, reminder flow, and AI features
- Contributed to the buildathon demo preparation and presentation strategy
- Reviewed the PRD and technical documentation for clarity and completeness

---

### 👩‍🔬 Winnie — Data Scientist & Backend Logic

**Role:** Data Scientist, Analytics Engineer

**Contributions:**
- Designed the analytics and insights engine — defined the logic for client reliability scores, monthly income calculations, and average payment days
- Developed the rule-based payment risk prediction model (Low / Medium / High) based on client payment behaviour patterns
- Defined the data schema for the invoices and users tables in Supabase/PostgreSQL
- Designed the Smart Payment Guard logic — overdue detection rules and due-soon alert thresholds
- Contributed to the AI feature specifications — defined the prompts and logic for the Claude API integrations
- Analysed the research data on African freelancer payment delays and contributed to the problem statement
- Reviewed the insights dashboard design and validated the accuracy of all financial metrics

---

### 👤 Elizabeth Edward — DevOps & Backend Engineer

**Role:** DevOps, Backend Integration

**Contributions:**
- Participated in initial team setup and discussions
- Contributed to planning for deployment and infrastructure setup

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React 18 + TypeScript |
| Styling | Tailwind CSS |
| Backend / Auth | Supabase (PostgreSQL + Auth) |
| AI Integration | Anthropic Claude API (claude-sonnet-4-20250514) |
| Payment API | Interswitch Web Checkout + BVN Identity + Transaction Search |
| Charts | Recharts |
| Icons | Lucide React |
| Fonts | Plus Jakarta Sans |
| Deployment | Lovable (live URL) |

---

## 🚀 How to Run Locally

```bash
# Clone the repository
git clone https://github.com/[your-github-username]/paytracka.git
cd paytracka

# Install dependencies
npm install

# Add environment variables
# Create a .env file with:
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
ANTHROPIC_API_KEY=your_anthropic_api_key

# Start the development server
npm run dev
```

---

## 🗄️ Database Schema

```sql
-- Users table
CREATE TABLE users (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  full_name VARCHAR(255) NOT NULL,
  email VARCHAR(255) UNIQUE NOT NULL,
  phone VARCHAR(20),
  bvn_verified BOOLEAN DEFAULT FALSE,
  created_at TIMESTAMP DEFAULT NOW()
);

-- Invoices table
CREATE TABLE invoices (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  invoice_ref VARCHAR(20) UNIQUE NOT NULL,
  user_id UUID REFERENCES users(id),
  client_name VARCHAR(255) NOT NULL,
  client_email VARCHAR(255),
  amount NUMERIC(12,2) NOT NULL,
  due_date DATE NOT NULL,
  payment_method VARCHAR(50),
  status VARCHAR(20) DEFAULT 'pending',
  description TEXT,
  payment_link TEXT,
  created_at TIMESTAMP DEFAULT NOW()
);
```

---

## 📱 Screens

1. **Splash + Onboarding** — 3-step value proposition slides
2. **Register / Login** — Supabase authentication with optional BVN verification
3. **Dashboard** — Hero summary card, quick actions, recent invoices
4. **Unified Inbox** — All transactions from all platforms
5. **Who Owes Me** — Kanban: Overdue | Due Soon | Paid
6. **Insights** — AI summary, income chart, client reliability, What If simulator
7. **Profile** — Identity Verified badge, settings, payment sources

---

## 📊 Success Metrics

| Metric | Target |
|---|---|
| Invoices created | 5+ per demo session |
| Payment links generated | 3+ working links |
| AI features demonstrated | 4 (reminder, risk, summary, description) |
| Interswitch APIs integrated | 3 (Web Checkout, BVN, Transaction Search) |
| Live URL accessible | ✅ Yes |

---

## 🔮 Future Enhancements (v2)

- Real-time Interswitch payment confirmation via webhooks
- Native Flutter mobile app (Android + iOS)
- Full bank and platform integrations (Upwork, Fiverr, Payoneer)
- Advanced ML payment risk scoring
- Multi-currency live exchange rates
- Automated payment imports

---

## 📄 Documentation

- [Product Requirements Document (PRD)(https://docs.google.com/document/d/1DDJ2zb7DVWz4wARXcomoZYa4Z6imVcOankh5Z_lKTTg/edit?usp=sharing)
- [Technical Documentation](https://docs.google.com/document/d/1FZcMLQgD8oo7SFljepadqvzkufraLVS2/edit?usp=sharing&ouid=117808902946980594183&rtpof=true&sd=true) 
- [API Contract](https://docs.google.com/document/d/1uu4LE_mfITXuRuBa2GWpD0vUWeAttKAf/edit?usp=sharing&ouid=117808902946980594183&rtpof=true&sd=true)

---

## 🏆 Buildathon Submission

- **Team Lead:** Okoro Oluchi Ruth
- **Live Link:** https://paytracka.lovable.app 
- **Submission:** Single submission by team lead
- **Category:** Fintech / Financial Inclusion

---

*Built with ❤️ for African freelancers — PayTracka, the app that ends payment chaos.*
