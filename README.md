# 🌿 VitaMate – AI Wellness Companion

**VitaMate** is a React Native mobile app that acts as your **empathetic AI wellness companion**, designed to hold natural, emotionally intelligent conversations — all **offline**.  
It helps users reflect, de-stress, and build positive habits through guided AI conversations.

---

## ✨ Features

- 🧠 **Conversational AI (Vita):** Custom-built rule-based logic system that generates natural, empathetic replies.  
- 💾 **Offline-First:** Entire AI logic runs locally — no server or API calls.  
- 🗣️ **Voice Input:** Integrated speech-to-text using `expo-voice` for hands-free journaling.  
- 🧘 **Guided Reflection Flows:** JSON-defined “interventions” for wellness techniques (like mindfulness & stress relief).  
- 🧩 **Context Memory:** Vita remembers previous chats and follows up later using short-term and long-term memory.  
- 🧭 **Safety System:** Detects crisis/self-harm language and responds with safe, supportive fallback messages.  
- 🌗 **Dynamic Theming:** Light/Dark mode with context-based theming.  
- ⚡ **Optimized Architecture:** Modular AI pipeline for easy extension and debugging.  

---

## 🧩 Tech Stack

| Layer | Technologies |
|-------|---------------|
| **Frontend** | React Native (Expo), React Navigation, AsyncStorage |
| **AI Engine** | Custom JS logic modules (`utils/logic/`) |
| **Speech Recognition** | Expo Voice / Native Voice APIs |
| **State Management** | React Context API |
| **Styling** | Custom theme system (`ThemeContext.js`, `Theme.js`) |
| **Testing** | Node CLI test harness (`utils/testHarness.js`) |

---

## 🗂️ Folder Structure

```text
VitaMate/
│
├── screens/
│   └── ConversationScreen.js           # Chat UI and input logic
│
├── utils/
│   ├── conversationLogic.js            # Entry point for AI logic
│   ├── logic/
│   │   ├── controller.js               # Main orchestration pipeline
│   │   ├── composer.js                 # Empathetic reply generation
│   │   ├── detectors.js                # Keyword & intent detection
│   │   ├── memory.js                   # Short & long-term memory
│   │   ├── flow.js                     # Guided technique flows
│   │   ├── safety.js                   # Crisis detection and filters
│   │   ├── state.js                    # Conversation state manager
│   │   ├── utils.js                    # NLP utilities & helpers
│   │   └── data.js                     # Loads JSON-based response logic
│   └── testHarness.js                  # CLI test for AI pipeline
│
├── context/
│   ├── ThemeContext.js
│   └── DataContext.js
│
├── constants/
│   └── Theme.js
│
└── App.js
```

---

## 🚀 Run Instructions

### 🧰 Prerequisites
- Node.js ≥ 18  
- Expo CLI installed globally:
  ```bash
  npm install -g expo-cli
  ```

### 🪄 Setup Steps

**1️⃣ Clone the repository**
```bash
git clone https://github.com/SparshSingh700/VitaMate.git
cd VitaMate
```

**2️⃣ Install dependencies**
```bash
npm install
```

**3️⃣ Start the Expo development server**
```bash
npx expo start
```

**4️⃣ Run on device or emulator**
- Press `a` → Android emulator  
- Press `i` → iOS simulator  
- Or scan the QR code using **Expo Go** on your phone  

---

## 🧪 Test the AI Logic (Node CLI)

You can simulate the AI engine without running the app:

```bash
node utils/testHarness.js
```

**Example output:**
```text
User: I'm feeling really stressed with exams coming up
AI: I hear you. That makes sense. Do you want to tell me more about it?
----
User: Yes
AI: Let's try this. What usually helps you relax?
```

---

## 📱 Demo Preview

| Feature | Description |
|----------|-------------|
| 🗣️ **Voice Input** | Speak instead of typing |
| 💬 **Empathetic Replies** | Vita responds with warmth and validation |
| 🧘 **Guided Techniques** | Includes mindfulness & stress-relief flows |
| 🔒 **Safety Layer** | Detects and responds to crisis inputs |
| 💾 **Offline AI** | No server — pure local logic engine |

---

## 🛡️ Safety and Ethics

> ⚠️ VitaMate is **not a substitute for professional mental health care**.  
> It includes safety checks for crisis phrases and recommends reaching out to professional help services if needed.

---

## 👨‍💻 Author

**Sparsh Singh**  
🎓 B.Tech CSE Final Year Project – AI Wellness Companion  
📍 India  
🔗 [GitHub Profile](https://github.com/SparshSingh700)

---

## 💡 Future Scope

- [ ] Integrate LLM-based hybrid mode (local + API fallback)  
- [ ] Add journaling analytics (sentiment trends)  
- [ ] Implement daily mood tracking dashboard  
- [ ] Add push reminders for mindfulness breaks  

---

## 🧭 License

This project is for **educational and research purposes** only.  
All rights reserved © 2025 **Sparsh Singh**.
