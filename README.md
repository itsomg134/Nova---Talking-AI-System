#  Nova - Talking AI System

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Made with JavaScript](https://img.shields.io/badge/Made%20with-JavaScript-1f425f.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Web Speech API](https://img.shields.io/badge/Web%20Speech-API-blue.svg)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API)

<div align="center">
  <img src="https://img.shields.io/badge/AI-Powered-ff69b4.svg" alt="AI Powered">
  <img src="https://img.shields.io/badge/Voice-Enabled-success.svg" alt="Voice Enabled">
  <img src="https://img.shields.io/badge/Responsive-Design-brightgreen.svg" alt="Responsive">
</div>

<br>

> **Nova** is an intelligent, voice-enabled AI assistant that brings conversations to life. With a sleek, futuristic interface and real-time speech capabilities, Nova can both understand your voice and respond with natural speech — creating a truly interactive experience.

##  Features

###  Core Capabilities
- ** Text Chat** - Type your messages and get intelligent AI responses
- ** Voice Input** - Speak naturally using your microphone (Web Speech API)
- ** Voice Output** - Nova speaks back with Text-to-Speech synthesis
- **Smart Responses** - Context-aware replies with personality
- **Modern UI** - Glass-morphism design with smooth animations

###  Interactive Elements
- Real-time typing indicators
- Message history with user/AI distinction
- Toggle voice replies on/off
- Responsive design for all devices
- Gradient accents and glow effects

<img width="1902" height="1277" alt="image" src="https://github.com/user-attachments/assets/9c828813-c220-4866-8490-57cd2ed246a7" />


### Voice Interaction Flow
1.  Click the microphone button
2.  Speak your question naturally
3.  Nova transcribes and processes
4.  Receive both text and voice response

##  Technologies Used

| Technology | Purpose |
|------------|---------|
| **HTML5** | Structure & semantics |
| **CSS3** | Modern styling, gradients, animations |
| **JavaScript (ES6+)** | Core logic & interactions |
| **Web Speech API** | Speech recognition & synthesis |
| **Font Awesome 6** | Icon system |
| **Google Fonts** | Inter typeface |

##  Installation

### Quick Start
Simply clone the repository and open `index.html` in your browser:

```bash
# Clone the repository
git clone https://github.com/yourusername/nova-talking-ai.git

# Navigate to project directory
cd nova-talking-ai

# Open in browser (macOS)
open index.html

# Or on Windows
start index.html
```

### Local Server (Recommended)
For best performance, run a local development server:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Then visit http://localhost:8000
```

##  Usage Guide

###  Text Mode
1. Type your message in the input field
2. Press Enter or click the send button
3. Nova will respond with text and optional voice

###  Voice Mode
1. Click the **"Start talking"** button in the Voice Panel
2. Allow microphone access when prompted
3. Speak clearly (English recommended)
4. Wait for Nova to process and respond

###  Voice Reply Toggle
- Check **"Enable Nova's voice replies"** to hear spoken responses
- Uncheck to receive only text responses

##  AI Response Categories

Nova understands and responds to various topics:

| Category | Example |
|----------|---------|
| Greetings | "Hello", "Hi Nova" |
| Jokes | "Tell me a joke" |
| Emotions | "I feel sad today" |
| Questions | "What can you do?" |
| Time | "What time is it?" |
| Farewell | "Goodbye" |
| General Chat | Any casual conversation |

##  Browser Compatibility

| Browser | Support |
|---------|---------|
| Chrome |  Full Support |
| Edge |  Full Support |
| Safari |  Partial (TTS works, Speech Recognition limited) |
| Firefox |  Limited (Speech Recognition may require flag) |
| Opera |  Full Support |

> **Note**: Speech Recognition works best in Chromium-based browsers (Chrome, Edge, Brave).

##  Customization

### Modify AI Personality
Edit the `getNovaReply()` function in the JavaScript section to change Nova's responses:

```javascript
function getNovaReply(userMessage) {
  // Add custom responses
  if (userMessage.includes('your custom trigger')) {
    return "Your custom response here!";
  }
  // ... rest of the logic
}
```

### Change Visual Theme
Adjust CSS variables in the `:root` section:

```css
:root {
  --primary-gradient: linear-gradient(135deg, #7aa2f7, #bb9af7);
  --bg-dark: #0a0f1e;
  --accent-blue: #5f9eff;
  /* Add your custom colors */
}
```

##  Project Structure

```
nova-talking-ai/
│
├── index.html          # Main application file
├── README.md           # Documentation
├── LICENSE             # MIT License
└── assets/            # (Optional) Images, icons, etc.
```

##  Advanced Configuration

### Adding Custom Voices
```javascript
// Select specific voices
const voices = window.speechSynthesis.getVoices();
const customVoice = voices.find(v => v.name === 'Your Preferred Voice');
if (customVoice) utterance.voice = customVoice;
```

### Language Support
Modify the recognition language:
```javascript
recognition.lang = 'en-US'; // Change to 'es-ES', 'fr-FR', etc.
```

##  Contributing

Contributions are welcome! Here's how you can help:

1.  Fork the repository
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

### Ideas for Improvement
- Add conversation memory/context
- Integrate with GPT API for smarter responses
- Add multiple language support
- Save chat history in localStorage
- Add dark/light theme toggle
- Implement voice activity detection

##  License

Distributed under the MIT License. See `LICENSE` file for more information.

##  Acknowledgments

- [Web Speech API Documentation](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API)
- [Font Awesome](https://fontawesome.com/) for beautiful icons
- [Google Fonts](https://fonts.google.com/) for Inter typeface
- Inspired by modern AI assistants like Jarvis and ChatGPT

##  Contact & Support
