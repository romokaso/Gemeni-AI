<div align="center">

# 🤖 Gemini AI Assistant for Roblox

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Roblox](https://img.shields.io/badge/Roblox-Executor-red)](https://www.roblox.com/)
[![Lua](https://img.shields.io/badge/Lua-5.1-blue)](https://www.lua.org/)
[![Google AI](https://img.shields.io/badge/Google-Gemini%20API-4285F4)](https://ai.google.dev/)

**Powerful AI Assistant for Roblox with full Google Gemini API integration**

[📥 Installation](#-installation) • [🎮 Usage](#-usage) • [✨ Features](#-features) • [🔑 API Key](#-getting-api-key)

</div>

---

## 📋 Table of Contents

- [✨ Features](#-features)
- [📥 Installation](#-installation)
- [🔑 Getting API Key](#-getting-api-key)
- [🎮 Usage](#-usage)
- [🤖 Available Models](#-available-models)
- [🌐 Supported Languages](#-supported-languages)
- [⚙️ System Requirements](#️-system-requirements)
- [🔧 Troubleshooting](#-troubleshooting)
- [📸 Screenshots](#-screenshots)
- [🤝 Contributing](#-contributing)
- [📝 License](#-license)
- [📈 Changelog](#-changelog)

---

## ✨ Features

<table>
<tr>
<td width="50%">

### 🧠 Artificial Intelligence
- **23 Gemini models** — from lightweight to most powerful
- **Contextual memory** — AI remembers the entire conversation
- **Smart responses** — help with code, advice, problem solving
- **Instant answers** — fast request processing

</td>
<td width="50%">

### 💬 Chat
- **Reply, Regenerate, Edit, Stop** — full message control
- **Fast typing animation + timer**
- **Thinking dots** while AI generates
- **Code blocks** — copy with one click, run directly
- **Edit messages** after sending

</td>
</tr>
<tr>
<td width="50%">

### 🎨 Interface
- **Modern design** — stylish and user-friendly UI
- **2 themes** — dark and light
- **Smooth animations** — pleasant experience
- **Drag & Drop button** — move it anywhere
- **Hotkey** — press **Right Ctrl** to open/close the GUI

</td>
<td width="50%">

### 📂 History
- **Chat history** — save all conversations
- **Search** chats & messages
- **Pin chats** to the top of history
- **Preview, date and model** shown for each chat
- **Rename chats** and highlight messages

</td>
</tr>
<tr>
<td width="50%">

### 🔑 API
- **Multiple API keys** — easy switching
- **Auto-switch model** on any API error
- **Key verification** before saving
- **How to get key** guide built into the script

</td>
<td width="50%">

### 💾 Functionality
- **Auto-save** — settings, chats and drafts never lost
- **Draft saving** — unfinished messages are preserved
- **Copy text** — with one click
- **Sound effects** and notifications

</td>
</tr>
<tr>
<td width="50%">

### 🌍 Localization
- **10 interface languages** — English, Russian and more
- **Full translation** — entire interface
- **Quick switch** — in settings
- **Language remembered** after restart

</td>
<td width="50%">

### 🛡️ Reliability
- **Error handling** — auto-switches model on failures
- **Script errors auto-copy to clipboard**
- **Unexpected format protection**
- **Minimal RAM usage**

</td>
</tr>
</table>

---

## 📥 Installation

### 🚀 Method 1: Loadstring (Recommended)

Copy and execute in any Roblox Executor:

```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/romokaso/Gemeni-AI/main/Gemini-AI"))()
```

### 📋 Method 2: Manual Installation

1. Open the script file: [`Gemini-AI`](https://github.com/romokaso/Gemeni-AI/blob/main/Gemini-AI)
2. Click the **Raw** button in the top right corner
3. Copy all code (Ctrl+A → Ctrl+C)
4. Paste into your Executor
5. Click **Execute / Inject**

### ⚡ Method 3: With Error Handling

```lua
local success, err = pcall(function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/romokaso/Gemeni-AI/main/Gemini-AI"))()
end)

if not success then
    warn("❌ Error loading Gemini AI:", err)
end
```

---

## 🔑 Getting API Key

> ⚠️ **IMPORTANT:** Without an API key the script **WILL NOT work**! It's free and takes 2 minutes.

### 📝 Step-by-step guide

1. **Open Google AI Studio**
   Go to: <https://aistudio.google.com/apikey>

2. **Sign in**
   Click **Sign in** in the top right corner and sign in with your Google account. If you don't have an account — create one (free).

3. **Create API Key**
   Click the blue **"Create API Key"** button, select an existing project or create a new one, wait a few seconds.

4. **Copy the key**
   Your API key will appear (starts with `AIza...`). Click **Copy** or select and copy manually. **DON'T SHARE your key with others!**

5. **Paste in script**
   Launch the script in Roblox, paste the key in the window that appears, click **Confirm**. Done! ✅

> 💡 **Quick link:** <https://aistudio.google.com/apikey>

---

## 🎮 Usage

### 🎯 First Launch

1. Launch the script via loadstring or manually
2. Enter your API key in the window that appears
3. Click **Confirm** — the key will be saved automatically
4. The button appears in the top left corner of the screen
5. Click the button to open the chat

### 🖱️ Controls

| Action | Description |
| --- | --- |
| Click button | Open / close interface |
| Drag button | Move it to a convenient place |
| 📂 History | View, search, pin and rename saved chats |
| ⚙️ Settings | Change theme, language, API key |
| 🤖 Model | Select Gemini model (23 options) |
| ➖ Minimize | Minimize the window |
| ❌ Close | Close interface (return to key selection) |

### ⌨️ Hotkeys

| Key | Action |
| --- | --- |
| **Right Ctrl** | Open / close the GUI |
| **Enter** (in input field) | Send message |
| Copy button under message | Copy to clipboard |
| ▼ button (bottom right) | Scroll down |

### 💬 Usage Examples

> 👤 **You:** Write a teleport script for Roblox
> 🤖 **AI:** Sure! Here's an example teleport script...

> 👤 **You:** How to solve equation x² + 5x + 6 = 0?
> 🤖 **AI:** Let's solve this quadratic equation using the discriminant...

> 👤 **You:** Translate "Hello World" to Japanese
> 🤖 **AI:** "Hello World" in Japanese is: こんにちは世界...

> 👤 **You:** Come up with a name for my space game
> 🤖 **AI:** Here are some ideas for a space game...

---

## 🤖 Available Models

All **23 Gemini models** supported by the script:

### 🏆 Pro Models (Most Powerful)
Best for complex tasks, programming, analysis

| Model | Model ID |
| --- | --- |
| ✨ Gemini 3.1 Pro CustomTools | `gemini-3.1-pro-preview-customtools` |
| ✨ Gemini 3.1 Pro | `gemini-3.1-pro-preview` |
| 🔬 Deep Research Pro | `deep-research-pro-preview-12-2025` |
| 💎 Gemini 3 Pro | `gemini-3-pro-preview` |
| 🌟 Gemini 2.5 Pro | `gemini-2.5-pro` |
| 🎯 Gemini Pro Latest | `gemini-pro-latest` |

### ⚡ Flash Models (Fast)
Balance of speed and quality for everyday tasks

| Model | Model ID |
| --- | --- |
| 🚀 Gemini 3 Flash | `gemini-3-flash-preview` |
| ⭐ Gemini 2.5 Flash | `gemini-2.5-flash` |
| 🌙 Gemini 2.5 Flash Lite Preview | `gemini-2.5-flash-lite-preview-09-2025` |
| 🌙 Gemini 2.5 Flash Lite | `gemini-2.5-flash-lite` |
| 📌 Gemini Flash Latest | `gemini-flash-latest` |
| 📍 Gemini Flash Lite Latest | `gemini-flash-lite-latest` |
| 🔷 Gemini 2.0 Flash 001 | `gemini-2.0-flash-001` |
| 🔷 Gemini 2.0 Flash | `gemini-2.0-flash` |
| 💠 Gemini 2.0 Flash Lite 001 | `gemini-2.0-flash-lite-001` |
| 💠 Gemini 2.0 Flash Lite | `gemini-2.0-flash-lite` |

### 🧪 Experimental
Test and special models

| Model | Model ID |
| --- | --- |
| 🍌 Nano Banana Pro | `nano-banana-pro-preview` |

### 🎨 Gemma Models (Open Source)
Open models of different sizes

| Model | Model ID |
| --- | --- |
| 🦾 Gemma 3 27B | `gemma-3-27b-it` |
| 💪 Gemma 3 12B | `gemma-3-12b-it` |
| 👍 Gemma 3 4B | `gemma-3-4b-it` |
| 🤏 Gemma 3 1B | `gemma-3-1b-it` |
| 🔹 Gemma 3N E4B | `gemma-3n-e4b-it` |
| 🔹 Gemma 3N E2B | `gemma-3n-e2b-it` |

### 📊 Model Comparison

| Model | Speed | Quality | Use Case |
| --- | --- | --- | --- |
| Pro | 🐢 Slow | ⭐⭐⭐⭐⭐ | Complex tasks, code |
| Flash | ⚡ Fast | ⭐⭐⭐⭐ | Daily conversations |
| Lite | 🚀 Very fast | ⭐⭐⭐ | Simple questions |

---

## 🌐 Supported Languages

Full interface translation in **10 languages**:

| 🌍 Language | Code |
| --- | --- |
| English | `en` |
| Русский | `ru` |
| Українська | `uk` |
| Español | `es` |
| Français | `fr` |
| Deutsch | `de` |
| Italiano | `it` |
| Português | `pt` |
| Nederlands | `nl` |
| Polski | `pl` |

### 🔄 How to change language?

1. Open **Settings** (⚙️)
2. Click on the current language
3. Select the desired language from the list
4. The language changes instantly!

---

## ⚙️ System Requirements

### ✅ Required Executor Functions

Your executor MUST support:

| Function | Purpose |
| --- | --- |
| `request()` or `http_request()` | API requests |
| `readfile()` | Reading saved data |
| `writefile()` | Saving settings |
| `isfile()` | File checking |
| `setclipboard()` | Text copying |

### 🎮 Compatible Executors

Tested and works on:

| Executor | Status | Note |
| --- | --- | --- |
| ✅ Synapse X | Works | Full support |
| ✅ Script-Ware | Works | Full support |
| ✅ KRNL | Works | Full support |
| ✅ Fluxus | Works | Full support |
| ✅ Electron | Works | Full support |
| ✅ Arceus X | Works | Full support |
| ⚠️ JJSploit | Partial | Saving may not work |
| ❌ Old executors | Doesn't work | No HTTP support |

### 💻 Technical Specifications

| Spec | Value |
| --- | --- |
| 📝 Language | Lua 5.1 |
| 🔌 API | Google Gemini Generative Language API |
| 🎨 UI | Custom Roblox Instance |
| 💾 Data format | JSON (`GeminiAI_Data.json`) |
| 📦 Script size | ~740 lines / ~110 KB |
| 🚀 RAM required | Minimal |

---

## 🔧 Troubleshooting

### ❌ Script doesn't start

- Check your executor — make sure it supports HTTP
- Enable HttpService in game settings (if possible)
- Try another executor from the compatible list
- Restart Roblox and try again
- Check your internet connection

### 🔑 "Invalid API Key" / "API Error 400"

- **Check the key:**
  - Must start with `AIza`
  - Copied completely (usually ~39 characters)
  - No spaces at the start/end
- **Get a new key:**
  - Go to <https://aistudio.google.com/apikey>
  - Create a new API key
  - Paste it in the script
- **Check limits:** new keys have request limits — wait a few minutes if exceeded

### ⏱️ "Rate limit reached" / Error 429

- **What is this?** You exceeded the API request limit
- **Automatic solution:** the script will auto-switch to another model — just wait for the message
- **Manual solution:**
  - Wait 1–2 minutes
  - Add a new API key in settings
  - Switch to a Lite model (fewer limits)

> ℹ️ **Gemini API free tier limits:** roughly 10–15 requests per minute and up to ~1,500 requests per day for Flash models (Pro models have much lower daily caps). Limits vary by model and change over time — check the official [rate limits page](https://ai.google.dev/gemini-api/docs/rate-limits) for current numbers.

### 💾 Chat history doesn't save

- **Check executor functions:**
  ```lua
  print(writefile) -- Should output: function
  print(readfile)  -- Should output: function
  ```
- **Write permissions:** some executors require permissions — check executor settings
- **Try another executor:** JJSploit often doesn't support saving — use KRNL, Fluxus or others
- **Clear cache:** delete the `GeminiAI_Data.json` file (if it exists) and restart the script

### 🖼️ Button doesn't appear

- Wait for loading — may take 5–10 seconds
- Check other corners — the button might be off-screen
- Restart the script
- Check the console for errors (F9 in Roblox)

### 🌐 Language/theme doesn't change

This is normal! When changing language or theme:
- The GUI is completely recreated
- You return to the main screen
- This is done for proper application of changes

Your data is saved: chat history ✅, API keys ✅, selected model ✅

### 📱 Other Issues

| Problem | Solution |
| --- | --- |
| AI responds in English instead of another language | Language in settings affects only the UI, not AI responses. For responses in your language, write in that language! |
| Takes long to respond / no response | Pro models think longer. Switch to Flash or Lite model |
| "Unexpected response format" error | Try another model — some experimental models are unstable |
| Script closes when clicking ❌ | This is normal! ❌ closes the GUI and returns to API key input. Use ➖ to minimize |

### 💬 Need Help?

If the problem is not solved:
- 📝 Open an [Issue](https://github.com/romokaso/Gemeni-AI/issues)
- 📋 Describe the problem in detail
- 📎 Attach an error screenshot (if any)
- 💻 Specify your executor

---

## 📸 Screenshots

| | |
| --- | --- |
| 🌙 Dark Theme | Screenshots will be added later |
| ☀️ Light Theme | Screenshots will be added later |
| ⚙️ Settings | Screenshots will be added later |
| 📂 Chat History | Screenshots will be added later |

---

## 🤝 Contributing

Want to help improve Gemini AI? Any contribution is welcome!

### 🐛 Report a bug

Found a bug?
1. Open an [Issue](https://github.com/romokaso/Gemeni-AI/issues)
2. Describe the problem
3. Attach a screenshot

### 💡 Suggest a feature

Have a feature idea?
1. Open an [Issue](https://github.com/romokaso/Gemeni-AI/issues)
2. Describe the feature
3. Explain why it's needed

### 🌍 Add a translation

Know another language?
1. Fork the repository
2. Add the translation
3. Open a Pull Request

### 📝 How to make a Pull Request

1. Fork the repository (click **Fork** in the top right corner)
2. Clone your fork:
   ```bash
   git clone https://github.com/YOUR_USERNAME/Gemeni-AI.git
   ```
3. Create a branch:
   ```bash
   git checkout -b feature/amazing-feature
   ```
4. Make changes and commit:
   ```bash
   git commit -m "Add amazing feature"
   ```
5. Push to your branch:
   ```bash
   git push origin feature/amazing-feature
   ```
6. Open a Pull Request on GitHub

### 📜 Rules

- ✅ Follow the project code style
- ✅ Test changes before PR
- ✅ Describe what changed and why
- ❌ Don't add malicious code
- ❌ Don't steal user API keys

---

## 📝 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file.

With the MIT License you can:

- ✅ Use commercially
- ✅ Modify code
- ✅ Distribute
- ✅ Use privately
- ✅ Create forks

BUT you must:

- ⚠️ Include a copy of the license
- ⚠️ Credit the original author

### ⚠️ Disclaimer

**IMPORTANT! Read before using:**

- 📚 This project was created for educational purposes
- ⚖️ The author is not responsible for your use of the script
- ⚠️ The author is not responsible for Roblox bans

By using this script you agree to these terms!

---

## 📈 Changelog

### 🆕 Latest Update (March 2026)

**❌ Deleted**
- Gemini Exp 1206 (not working)
- Gemini 2.5 Flash Preview (not working)

**🤖 New Models**
- Gemini 3.1 Pro CustomTools
- Gemini 3.1 Pro

**📌 New Features**
- Pin chats to the top of history
- Auto-switch model on any API error
- Stop generation shows a stopped message
- Draft saving
- Script errors auto-copy to clipboard

**🌍 Languages**
- 194 languages
- Language search

**✨ Chat**
- Reply, Regen, Edit, Stop
- Fast typing + timer
- Code blocks: copy + run
- Thinking dots
- Edit messages

**🔍 History**
- Search chats & messages
- Preview, date, model
- Message highlight

**⌨️ Hotkey**
- Right Ctrl — open/close

**🔑 API**
- Multiple keys
- Switch / Add / Delete

**📋 Other**
- Sound, timer, drafts

### v1.0.0 (February 17, 2025)

- ✨ First public release
- 🧠 Support for 23 Gemini models
- 🌍 10 interface languages
- 💾 Chat history system
- 🔑 Multiple API key management
- 🎨 Dark and light theme
- 🖱️ Drag & Drop button
- 💾 Auto-save settings
- 📋 Message copying

---

## 👤 Author

**[romokaso](https://github.com/romokaso)** — [Gemeni-AI](https://github.com/romokaso/Gemeni-AI)

Made with ❤️ for the Roblox Community

### 🌟 Support the Project

If the project helped you or you liked it:

- ⭐ **Star the repo** — helps others find the project
- 🔄 **Fork it** — create your own version
- 📢 **Tell friends** — share the link
- 💬 **Leave feedback** — write what you think

### 📞 Contact

Have questions? Contact me:

- 📧 GitHub Issues: [Create Issue](https://github.com/romokaso/Gemeni-AI/issues)
- 💬 Discussions: [Discussions](https://github.com/romokaso/Gemeni-AI/discussions)
- 🐛 Bug Reports: [Report Bug](https://github.com/romokaso/Gemeni-AI/issues/new)

---

🎉 **Thank you for using Gemini AI!**

Made with ❤️ for the Roblox Community

⬆ [Back to top](#-gemini-ai-assistant-for-roblox)
