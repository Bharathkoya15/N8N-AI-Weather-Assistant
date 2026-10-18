# 🌦️ AI Daily Weather Assistant (n8n + Google Gemini)

An automated daily workflow built in **n8n** that fetches real-time weather data and uses **Google Gemini** to generate a personalized morning email with outfit suggestions, outdoor activity ideas, and practical weather reminders.

## ⚙️ How It Works
1. **Schedule Trigger:** Runs automatically every morning at 9:00 AM.
2. **HTTP Request (OpenWeatherMap API):** Fetches live temperature, weather description, and humidity data.
3. **Basic LLM Chain (Google Gemini 3.1 Flash Lite):** Analyzes the weather metrics and drafts a friendly, under-100-word daily plan.
4. **Gmail Node:** Sends the personalized plan straight to the user's inbox.

## 🚀 How to Use This Workflow
1. Download the `open weather.json` file from this repository.
2. Open your **n8n** workspace, click the menu icon, and select **Import from File**.
3. Add your own **OpenWeatherMap API key** in the HTTP Request node.
4. Connect your **Google Gemini API** and **Gmail OAuth2** credentials.
5. Activate the workflow!
