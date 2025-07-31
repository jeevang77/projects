
#  Spidey Voice Assistant

Spidey is a Python-based voice assistant that listens to your voice commands and performs tasks like web searches, YouTube queries, location lookups, checking stock prices, and more — all through natural conversation.

---

##  Features

-  Google search from your voice input  
- 📺 YouTube search and play  
- 🗺️ Location lookup on Google Maps  
- 📈 Stock price checker using [Yahoo Finance](https://pypi.org/project/yfinance/)  
- 🕒 Time announcements  
- 🗣️ Basic conversation and name memory  
- 👋 Friendly exit commands like "bye", "see you", etc.

---

##  How It Works

1. Captures voice input using your microphone.
2. Converts it to text using Google's Speech Recognition API.
3. Detects intent using keywords.
4. Executes relevant actions using Python tools and APIs.

---

##  Setup Instructions

###  Step 1: Create and Activate a Virtual Environment (Recommended)

```bash
# Windows
python -m venv myenv
myenv\Scripts\activate

# macOS/Linux
python3 -m venv myenv
source myenv/bin/activate
```

###  Step 2: Install Required Packages

#### Option A: Automatic Installation

```bash
pip install -r requirements.txt
```

#### Option B: Manual Installation

Use this if `requirements.txt` doesn't work:

```bash
pip install SpeechRecognition
pip install gTTS
pip install playsound
pip install yfinance
pip install pyaudio
```

If you face issues with `pyaudio` (especially on Windows):

```bash
pip install pipwin
pipwin install pyaudio
```

>  On macOS: Install PortAudio first with `brew install portaudio` then try `pip install pyaudio`.

---

##  How to Run

Run the assistant using the command:

```bash
python assistant.py
```

Make sure your mic is working and you're connected to the internet.

---

##  Libraries Used

| Library           | Purpose                            |
|------------------|-------------------------------------|
| `SpeechRecognition` | Capture voice input               |
| `gTTS`            | Text-to-speech (Google TTS)        |
| `playsound`       | Play spoken output audio           |
| `webbrowser`      | Open browser tabs                  |
| `yfinance`        | Fetch live stock prices            |
| `pyaudio`         | Enable microphone functionality    |

---

##  Example Voice Commands

| Action           | Say This...                                      |
|------------------|--------------------------------------------------|
| Google Search    | "Search for quantum computing"                   |
| YouTube Video    | "Play Spider-Man trailer on YouTube"             |
| Location Map     | "Where is the Eiffel Tower"                      |
| Stock Price      | "Tell me the stock price of Tesla"              |
| Ask Time         | "What's the time now?"                          |
| Set Name         | "My name is Peter"                              |
| Exit             | "Bye", "See you later", "Quit"                  |

---

##  Future Plans

- Add GPT-style conversational abilities.
- Integrate weather, reminders, and calendar access.
- Build a GUI using Tkinter or PyQt.
- Expand stock market coverage dynamically.

---

##  How It Works

1. Uses the `speech_recognition` library to capture and convert voice to text.
2. Matches input with predefined keyword sets to determine the user’s intent.
3. Executes corresponding actions using `webbrowser`, `yfinance`, and text-to-speech via `gTTS`.

---

##  Installation

# Create virtual environment
python -m venv myenv
source myenv/bin/activate  # On Windows: myenv\Scripts\activate

# Install required packages
pip install -r requirements.txt
