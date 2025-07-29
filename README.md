# 🔍 AI Research & Summarization Workflow (n8n)

This repository contains a fully automated **AI-powered workflow** built in [n8n](https://n8n.io/) that performs:

1. 📥 Receives a topic from the user (via chat or API)  
2. 🌐 Performs web-based research using **Google Gemini**  
3. 🧠 Summarizes the content using **OpenAI Chat Models (e.g., GPT-4)**  
4. 📄 Outputs the summary directly to **Google Docs**

---

## ⚙️ How It Works

flowchart LR

    A[User Sends Topic] --> B[Research Agent (Gemini)]
    B --> C[Summarize Agent (OpenAI)]
    C --> D[Google Docs - Save Summary]

---

### 🔧 Nodes Explained

| Node Name                  | Description                                                                 |
|----------------------------|-----------------------------------------------------------------------------|
| `When Chat Message Received` | Trigger that starts the workflow when a user submits a topic               |
| `Research Agent`           | Uses Google Gemini to gather relevant information based on the topic       |
| `Summarize Agent`          | Summarizes the research using OpenAI's language model                      |
| `Summarize Document`       | Updates/saves the final summary into Google Docs                           |

---

## 🚀 Use Cases

- AI newsletters & blog content automation  
- Research notes for students or analysts  
- Auto-generated study materials or reports  
- Content repurposing for social media

---

## 🧠 System Prompts

> Customizable prompts for both agents (Gemini & OpenAI) to define tone, output structure, and length.

📌 **[View Prompts PDF]**

---

## 📦 Requirements

- n8n (Self-hosted or Cloud)
- OpenAI API key
- Google Gemini API credentials
- Google Docs API integration in n8n

---

## 🛠️ Setup Instructions

1. Clone this repo  
2. Import the `.json` workflow into n8n  
3. Connect OpenAI, Gemini, and Google Docs credentials  
4. Update agent prompts (or use provided ones)  
5. Trigger via chat or webhook and test with a sample topic like:  
   `"Impact of Generative AI in Healthcare"`

---

## 🧪 Demo Screenshots

> ![Workflow Screenshot](assets/workflow.png)

> ![Google Doc Output](assets/google-docs-summary.png)

---

## 🤝 Contributing

Feel free to fork, improve, and submit PRs.  
Enhancements and feedback are welcome!

---

## 📄 License

MIT License — free for personal and commercial use with credit.

---

## 🙌 Credits

Built by **Vishnu S.R.** using:
- 🛠️ [n8n.io](https://n8n.io/)
- 🤖 [OpenAI](https://platform.openai.com/)
- 🌐 [Google Gemini](https://deepmind.google/technologies/gemini/)
