# n8n-automation-agents


# 🤖 AI News Bot — n8n Automation Workflow

An automated daily AI & Tech newsletter bot built with **n8n**, **Google Gemini**, and **Gmail**. Runs every morning at 10 AM, fetches the latest AI and tech news, formats it using AI, and delivers it straight to your inbox.

---

## 🚀 What It Does

Every day at **10:00 AM**, this workflow automatically:

1. 📡 Fetches **AI news** from [AI Business](https://aibusiness.com)
2. 💻 Fetches **Tech news** from [TechCrunch](https://techcrunch.com)
3. 🗓️ Fetches **Upcoming AI events in India** via SerpAPI
4. 🧠 Sends all data to **Google Gemini** to format into a clean newsletter
5. 📧 Delivers the newsletter to your **Gmail inbox**

---

## 📸 Workflow Overview

```
The image that i given in the below file Screenshot 2026-03-10 224914.png

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **n8n** | Workflow automation platform |
| **Google Gemini (PaLM API)** | AI formatting & summarization |
| **Gmail API** | Send the newsletter email |
| **SerpAPI** | Fetch upcoming AI events |
| **RSS Feed Reader** | Pull news from AI Business & TechCrunch |

---

## 📧 Sample Newsletter Output Format

```
Hi there,
Here's your Tech Brief:

AI NEWS HIGHLIGHTS
======================
HEADLINE IN ALL CAPS
Summary in 1–2 sentences.
Link: https://...

TECHNOLOGY UPDATES
======================
...

UPCOMING AI EVENTS
======================
...

— Your AI Intelligence Team
```

---

## ⚙️ Setup Instructions

### Prerequisites
- [n8n](https://n8n.io) installed (cloud or self-hosted)
- Google Gemini API key
- Gmail OAuth2 credentials configured in n8n
- SerpAPI key (free tier available at [serpapi.com](https://serpapi.com))

### Steps

1. **Clone this repo**
   ```bash
   git clone https://github.com/YOUR_USERNAME/ai-news-bot.git
   ```

2. **Import the workflow into n8n**
   - Open your n8n dashboard
   - Go to **Workflows → Import from File**
   - Select `AI_news_bot.json`

3. **Configure your credentials in n8n**
   - Add your **Google Gemini API** credentials
   - Add your **Gmail OAuth2** credentials
   - Add your **SerpAPI key** in the HTTP Request node

4. **Update the recipient email**
   - In the `Send a message` (Gmail) node, replace `YOUR_EMAIL@gmail.com` with your email

5. **Activate the workflow**
   - Toggle the workflow to **Active**
   - It will now run every day at 10:00 AM ✅

---

## 🔐 Security Note

> ⚠️ Never commit your real API keys to GitHub.  
> The `AI_news_bot.json` in this repo has all credentials replaced with placeholders like `YOUR_SERPAPI_KEY_HERE`.  
> Add your real keys only inside your n8n credential manager.

---

## 🙋‍♂️ Built By

**Thrishanth** — AI Automation Developer  
Skills: n8n · Prompt Engineering · HTML/CSS · Python · SQL  
📎 [LinkedIn](https://www.linkedin.com/in/thrishanth?utm_source=share_via&utm_content=profile&utm_medium=member_android)

---

## 📄 License

MIT License — feel free to use, modify, and share!
