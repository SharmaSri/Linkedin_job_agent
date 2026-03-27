# 🤖 AI Job Application Agent

An end-to-end **AI-powered job automation system** that searches jobs, generates tailored resumes, and sends personalized application emails automatically.

---

## 🚀 Overview

This project automates the entire job application pipeline:

```
Job Fetching → AI Resume Generation → AI Email Generation → Email Sending
```

It is designed for **AI/ML engineers, data scientists, and developers** who want to scale their job search efficiently.

---

## 🧠 Features

* 🔍 Automated job fetching (currently mocked, extendable to real sources)
* 📄 AI-generated tailored resumes for each job
* ✉️ Personalized job application emails
* 📬 Automatic email sending with resume attachment
* ⏱️ Scheduler for daily automation
* 🧩 Modular and extensible architecture

---

## 🏗️ Project Structure

```
ai-job-agent/
│
├── .venv/                     # Virtual environment
├── config/                   # Configurations & prompts
├── core/                     # Core pipeline logic
├── services/                 # External services (AI, email, file)
├── linkedin_mcp/             # Job fetching layer (currently mocked)
├── resume_templates/         # Base resume templates
├── generated_resumes/        # Generated resumes (PDF)
├── email_templates/          # Email templates
├── logs/                     # Logs
├── scripts/                  # Entry points
├── data/                     # Job data (optional)
├── .env                      # Environment variables
├── requirements.txt
└── README.md
```

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository

```
git clone https://github.com/your-username/ai-job-agent.git
cd ai-job-agent
```

---

### 2️⃣ Create Virtual Environment

```
uv venv --python 3.11
```

Activate:

```
.\.venv\Scripts\activate
```

---

### 3️⃣ Install Dependencies

```
uv pip install -r requirements.txt
```

---

### 4️⃣ Configure Environment Variables

Create a `.env` file:

```
OPENAI_API_KEY=your_api_key
EMAIL=your_email@gmail.com
APP_PASSWORD=your_app_password
```

---

## 🔐 Gmail Setup (Important)

To send emails:

1. Enable **2-Step Verification**
2. Generate **App Password**
3. Use the app password in `.env`

---

## ▶️ Running the Application

### Run Once

```
python -m scripts.run_agent
```

---

### Run with Custom Query

```
python -m scripts.run_agent "AI Engineer India"
```

---

### Run with Scheduler

```
python -m scripts.scheduler
```

---

## ⚙️ How It Works

1. **Fetch Jobs**

   * Retrieves job listings (mocked or via integration)

2. **Generate Resume**

   * Uses AI to tailor resume based on job description

3. **Generate Email**

   * Creates a personalized application email

4. **Send Email**

   * Sends email with resume attachment via SMTP

---

## 📄 Example Output

* Generated Resume → `generated_resumes/resume_0.pdf`
* Email sent to recruiter automatically

---

## ⚠️ Limitations

* Job data is currently mocked
* LinkedIn scraping is restricted
* Not all job postings contain recruiter emails
* Gmail sending limits apply (~100 emails/day)

---

## 🔮 Future Enhancements

* 🔗 Real job scraping integration (LinkedIn, APIs)
* 🧠 Job matching & scoring (AI-based filtering)
* 👤 Recruiter discovery & outreach
* 💬 LinkedIn message automation
* 📊 Application tracking dashboard
* ⚡ Parallel job applications (scaling)

---

## 🛠️ Tech Stack

* Python 3.11
* OpenAI / Gemini API
* SMTP (Gmail)
* FPDF (PDF generation)
* Schedule (automation)

---

## 💡 Use Case

* Automate job applications at scale
* Save time on repetitive tasks
* Increase response rate with personalized applications

---

## ⚠️ Disclaimer

* Use responsibly and avoid spamming recruiters
* Respect platform policies (e.g., LinkedIn terms of service)

---

## 👨‍💻 Author

Built by an AI enthusiast focused on automation, machine learning, and intelligent systems.

---

## ⭐ Contributing

Contributions are welcome! Feel free to fork and improve the system.

---

## 📬 Contact

For questions or collaboration, reach out via email or LinkedIn.

---
