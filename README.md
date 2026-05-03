🏥 MediBot – AI Telemedicine Scheduler
MediBot is an AI-powered telemedicine assistant built as a single-page web application. It helps patients book appointments, check symptoms, find doctors, and manage health reminders — all from a clean, modern interface powered by Google Gemini AI.

✨ Features
💬 AI Chat — Conversational assistant powered by Gemini 2.5 Flash for medical queries, appointment guidance, and general health questions
🩺 Symptom Checker — Select from 16 common symptoms and receive an AI-generated analysis of possible conditions and recommended next steps
👨‍⚕️ Find Doctors — Browse available specialist doctors and book consultations
📅 Appointments — View and manage upcoming appointments; book new ones via a modal interface
🔔 Reminders — Track medication schedules, follow-up visits, lab tests, and other health-related reminders
📋 Health Records — Access and manage personal health history
⚙️ Settings — Configure preferences and manage your Gemini API key
🚀 Getting Started
Prerequisites
A modern web browser (Chrome, Firefox, Edge, Safari)
A Google Gemini API key — Get one here
Running the App
Download or clone this repository
Open chatbot.html in your web browser (no server required)
On first launch, a prompt will appear asking for your Gemini API key
Enter your key (starts with AIza...) and click 🚀 Launch MediBot
Your key is saved locally in your browser and never sent to any external server
Note: The app runs entirely in the browser. No backend or installation is needed.

🔑 API Key
MediBot uses the Google Gemini 2.5 Flash model via the Generative Language API.

Your API key is stored in localStorage under the key gemini_key
It is only sent directly to generativelanguage.googleapis.com
To reset or change your key, go to Settings within the app
🗂️ Project Structure
Chatbot/
└── chatbot.html       # Complete single-file application (HTML + CSS + JavaScript)
The entire application — UI, styling, and logic — is contained within a single HTML file for maximum portability.

🛠️ Tech Stack
Layer	Technology
Markup	HTML5
Styling	CSS3 with custom properties (variables)
Logic	Vanilla JavaScript (ES6+)
AI Model	Google Gemini 2.5 Flash
Fonts	Syne & DM Sans (Google Fonts)
Storage	Browser localStorage
🧠 How the AI Works
The chat and symptom checker both call the Gemini API directly from the browser:

Chat: Maintains a rolling conversation history (chatHistory) to support multi-turn dialogue. A system prompt configures MediBot as a medical assistant.
Symptom Checker: Takes selected symptoms and sends them to Gemini with a structured prompt, returning possible diagnoses and recommended specialist types.
Temperature: Set to 0.7 for balanced, informative responses
Max output tokens: 800 per response
⚠️ Disclaimer
MediBot is intended for informational purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment. Always consult a qualified healthcare provider for medical decisions.

📄 License
This project is open for personal and educational use. See your organization's policy for commercial deployment.

ional interaction.
