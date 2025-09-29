Jarvis AI Assistant 🤖🎤

A voice-activated personal assistant built in Python, powered by:

🎙️ Speech Recognition with Vosk

🗣️ Text-to-Speech with pyttsx3

🧠 AI Chat and summarization using OpenAI GPT models

🌐 Web automation (open Google, YouTube, LinkedIn, etc.)

⏰ Reminders

📄 Webpage summarizer

💻 System control (shutdown, restart, sleep, open apps)

⚡ Features

Wake word "Jarvis"

Open websites (Google, YouTube, LinkedIn, GitHub, Kaggle, Movies4U, etc.)

AI-powered Q&A (via OpenAI API)

Save and read reminders (reminders.txt)

Summarize articles/webpages with GPT

Launch apps (Notepad, Calculator, Camera)

System commands: shutdown, restart, sleep

🛠 Installation

Clone the repository

git clone https://github.com/your-username/Jarvis-AI-Assistant.git
cd Jarvis-AI-Assistant


Create and activate virtual environment

python -m venv venv
source venv/bin/activate     # macOS/Linux
venv\Scripts\activate        # Windows


Install dependencies

pip install -r requirements.txt


Download Vosk Model

Go to: Vosk Models

Download a suitable model (e.g., vosk-model-small-en-us-0.15)

Extract it into a folder named model/ inside the project root.
Final structure:

Jarvis-AI-Assistant/
├── model/
│   ├── am
│   ├── graph
│   ├── ivector
│   └── conf
├── main.py
├── requirements.txt
└── README.md


Set up OpenAI API Key

Get your API key from OpenAI
.

Replace "your-api-key-here" in the code with your actual key.

(Recommended: use an .env file and python-dotenv to avoid exposing secrets).

▶️ Usage

Run the assistant:

python main.py


Then say "Jarvis" to activate it.

Example Commands:

"Jarvis, open Google"

"Jarvis, set reminder finish project report"

"Jarvis, what are my reminders"

"Jarvis, summarize https://en.wikipedia.org/wiki/OpenAI
"

"Jarvis, shutdown"

"Jarvis, open calculator"

"Jarvis, ask What is quantum computing?"

📂 Project Structure
Jarvis-AI-Assistant/
├── model/             # Vosk speech recognition model (not in repo if too large)
├── reminders.txt      # Stores user reminders
├── main.py            # Main code
├── requirements.txt   # Python dependencies
└── README.md          # Documentation

⚠️ Notes

The model/ folder might be large. If so, don’t commit it to GitHub. Instead, provide a download link in the README.

Do not commit API keys (use .env instead).

Works best on Windows (due to system control commands like shutdown/sleep).

🚀 Future Improvements

Add GUI for better interaction.

Multi-language support.

More app integrations (Spotify, Gmail, WhatsApp).

Smarter reminder system with notifications.
