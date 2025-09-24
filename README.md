# VED – AI Personal Voice Assistant

*Ved* is an interactive AI voice assistant built with *Python* and the *ElevenLabs API*. It can engage in natural spoken conversations, answer questions, summarize information, and generate stories, providing a dynamic and user-friendly AI experience.

## Features
- Real-time voice conversation with AI
- Human-like text generation and speech output
- Customizable prompts and first messages
- Easy integration with Python and ElevenLabs API
- Callback functions for agent responses, user transcripts, and interruptions

## Prerequisites
- Python 3.9 or higher
- pip (Python package installer)
- ElevenLabs API account with valid API key

## Installation
1. Clone the repository:
bash
git clone https://github.com/himakshimann/Ved.git
cd ved


2. Install required Python packages:

pip install -r requirements.txt


3. Create a .env file in the root directory and store your API key and Agent ID:

API_KEY=your_elevenlabs_api_key_here
AGENT_ID=your_agent_id_here

Note: The .env file keeps sensitive information secure and allows your Python script to access the API credentials without hardcoding them.


4. Ensure the Python script loads the .env file using python-dotenv:

from dotenv import load_dotenv
import os

load_dotenv()
API_KEY = os.getenv("API_KEY")
AGENT_ID = os.getenv("AGENT_ID")


*Running the Assistant*

Run the main Python script:

python assistant.py

Speak to the assistant and it will respond in real-time using text-to-speech.

Callbacks in the script will print agent responses, truncated responses, and user transcripts in the console.


*Customization*

Adjust dynamic variables or conversation configuration to suit your use case.


*Future Improvements*

-Add multi-language support
-Integrate with task automation (reminders, web search)
-Expand multimedia output or integrate with smart devices
