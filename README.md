# 🤖 AI-Avature: Automated Avatar Video Generator

AI-Avature is a fully automated pipeline that creates avatar-based videos from trending topics and publishes them across multiple social media platforms using **n8n**, **HeyGen**, and **AI models**.

## 🚀 Features

- 🔍 **Topic Detection**: Automatically selects trending topics from **Twitter**
- ✍️ **Script Generation**: Uses OpenAI to generate a short script for the topic
- 🎥 **Video Generation**: Uses **HeyGen** to generate an AI avatar video
- 📤 **Auto Publishing**: Posts the final video to social media (LinkedIn, Instagram, etc.)
- ⚙️ Fully automated using **n8n workflows**

## 🛠️ Tech Stack

- [n8n](https://n8n.io/) – Workflow automation
- [HeyGen API](https://docs.heygen.com/) – AI avatar video generation
- [Twitter API](https://developer.twitter.com/) – Fetch trending topics
- [OpenAI API](https://platform.openai.com/) – Content/script generation
- Python – Utility scripts for text formatting, request handling
- Webhooks – Real-time triggering and syncing

## 📁 Project Structure

```

.
├── workflows/             # n8n workflow JSON exports
├── scripts/               # Python scripts for data cleaning and helpers
├── docs/                  # Setup guide and API reference
├── .env.example           # Example environment variables
└── README.md              # Project overview

````

## 🔧 Setup Instructions

1. **Clone the repository**  
   ```bash
   git clone https://github.com/alihassanml/AI-Avature.git
   cd AI-Avature
````

2. **Configure `.env`**
   Rename `.env.example` to `.env` and fill in the required API keys:

   * Twitter Bearer Token
   * OpenAI API Key
   * HeyGen API Key
   * Webhook URLs for social platforms

3. **Import n8n Workflows**

   * Open your [n8n instance](https://n8n.io/)
   * Import workflow JSONs from the `workflows/` folder

4. **Connect APIs and Test**

---

## 📺 Example Workflow

1. 📈 Detect trending topic from Twitter
2. 🧠 Generate video script using LLM (OpenAI)
3. 🎤 Create avatar video via HeyGen
4. 📲 Post to LinkedIn & Instagram

---

## 🧠 Author

**Ali Hassan**
🚀 Data Scientist | Automation Engineer
📫 [LinkedIn](https://www.linkedin.com/in/ali-hassanml/) | 🌐 \[Portfolio Coming Soon]

---

## 📄 License

This project is licensed under the MIT License.
