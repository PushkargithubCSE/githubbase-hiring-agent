# GitHub AI Career Agent 🚀

## 📌 Project Idea

GitHub AI Career Agent is an automated system that detects new followers on a GitHub profile, analyzes their public repositories and contributions using AI, and recommends relevant job or internship opportunities tailored to their skills.

The system acts as an intelligent bridge between developers and opportunities by using real-world coding activity instead of traditional resumes.

---

## ❓ Problem Statement

Traditional hiring relies heavily on resumes, which often fail to reflect a developer’s true capabilities.

Developers showcase their real skills through:
- Open-source contributions
- Personal projects
- Commit history
- Technical depth in repositories

However, this data is underutilized in hiring processes.

Additionally:
- Developers struggle to find relevant opportunities
- Recruiters struggle to evaluate GitHub profiles effectively

---

## 💡 Solution

This project builds an AI-powered agent that:

1. Detects new followers on a GitHub account
2. Fetches and analyzes their public GitHub data
3. Extracts skills, experience level, and domain expertise
4. Matches the user with relevant job/internship opportunities
5. Sends personalized recommendations via email (if available)

---

## ⚙️ Tech Stack

### Backend
- Python 3.11
- FastAPI (for API and structure)

### Data Collection
- GitHub REST API
- httpx (async HTTP requests)
- BeautifulSoup (job scraping)

### AI Layer
- OpenAI GPT models
- Prompt engineering for skill inference
- Structured JSON outputs

### Scheduling
- APScheduler (background tasks)

### Database
- SQLite / PostgreSQL
- SQLAlchemy ORM

### Email Delivery
- SMTP (Gmail / SendGrid)

---

## 🧠 System Architecture

Scheduler (poll followers)
↓
GitHub API (fetch user data)
↓
Profile Analyzer (LLM)
↓
Career Inference Agent
↓
Job Fetcher
↓
Job Matching Engine
↓
Email Sender

## 📂 Project Structure


project-root/
│
├── app/
│ ├── github_client.py
│ ├── profile_analyzer.py
│ ├── job_fetcher.py
│ ├── job_matcher.py
│ ├── email_sender.py
│ ├── scheduler.py
│ └── db.py
│
├── outputs/
├── run.py
├── requirements.txt
└── README.md


---

## 🚀 Features

- Automated detection of new GitHub followers
- Deep analysis of repositories and coding patterns
- AI-powered skill and role inference
- Personalized job recommendations
- Automated email delivery system

---

## 🌍 Significance & Impact

- Encourages merit-based hiring using real work instead of resumes
- Helps developers discover relevant opportunities
- Demonstrates practical use of AI agents in real-world workflows
- Bridges the gap between open-source activity and career growth

This project showcases how AI can make hiring smarter, more efficient, and more inclusive.

---

## ⚠️ Ethical Considerations

- Only public GitHub data is used
- Emails are sent only if publicly available
- Users can opt out of receiving recommendations

---

## 📜 License

This project is licensed under the MIT License.
