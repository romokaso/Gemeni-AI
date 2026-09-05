# Gemeni-AI
Gemini AI Assistant for Roblox
# 🤖 Gemini AI Assistant for Roblox

[

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

](https://opensource.org/licenses/MIT)
[

![Roblox](https://img.shields.io/badge/Roblox-Executor-red)

](https://www.roblox.com/)
[

![Lua](https://img.shields.io/badge/Lua-5.1-blue)

](https://www.lua.org/)
[

![Google AI](https://img.shields.io/badge/Google-Gemini%20API-4285F4)

](https://ai.google.dev/)

<div align="center">

# ⛔ DISCONNECTED

### The Gemini AI Assistant has been **fully disabled and removed** from this repository.

The `Gemini-AI` file no longer contains the assistant. It now plays a single
cinematic **"DISCONNECTED"** overlay in Roblox and then folds into a small idle
status badge. No API, no keys, no chat, no code execution.

[⛔ Current status](#-current-status--disconnected) • [🎬 What the script does now](#-what-the-script-does-now) • [🧾 Legacy documentation](#-legacy-documentation)

</div>



![Divider](https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif)



</div>

---

## 📋 Table of Contents

**Current script**

- [⛔ Current Status — DISCONNECTED](#-current-status--disconnected)
- [🎬 What the script does now](#-what-the-script-does-now)
- [⚙️ Configuration](#️-configuration)
- [🖥️ Requirements](#️-requirements)
- [🧾 Legacy Documentation](#-legacy-documentation)

<details>
<summary><b>Legacy assistant docs</b> — features, installation, usage (kept for history, no longer functional)</summary>

- [✨ Features](#-features)
- [📥 Installation](#-installation)
- [🔑 Getting API Key](#-getting-api-key)
- [🎮 Usage](#-usage)
- [🤖 Gemini Models](#-available-models)
- [🌐 Languages](#-supported-languages)
- [⚙️ Requirements](#️-system-requirements)
- [🔧 Troubleshooting](#-troubleshooting)
- [📸 Screenshots](#-screenshots)

</details>

**Repository**

- [🤝 Contributing](#-contributing)
- [📝 License](#-license)

---

---

## ⛔ Current Status — DISCONNECTED

<table>
<tr>
<td width="50%">

### ❌ Removed forever

- **All HTTP traffic** to `generativelanguage.googleapis.com`
- **API key input**, validation and the multi-key manager
- **`readfile` / `writefile`** persistence (`GeminiAI_Data.json`)
- **`loadstring()`** execution of AI generated code
- **Clipboard access**, the `RightControl` hotkey
- Chat UI, chat history, settings, themes, translations, sounds

</td>
<td width="50%">

### ✅ What is left

- A pure client-side **animation** (a `ScreenGui` and tweens)
- No network, no files, no execution, no input hooks
- No game modification of any kind
- Optional cleanup of what the old script left behind

</td>
</tr>
</table>

> ### 🔐 Security note
> The old assistant stored Gemini API keys **in plain text** in `GeminiAI_Data.json`
> inside your executor workspace. This version deletes that file on launch, but the
> keys may already have been exposed — **revoke them manually** at
> [aistudio.google.com/apikey](https://aistudio.google.com/apikey).

---

## 🎬 What the script does now

Running the file plays a one-shot shutdown cinematic (~12 s) and then leaves a
compact idle badge at the bottom of the screen:

| # | Moment | What happens |
|---|--------|--------------|
| 1 | `0.0 s` | Backdrop, vignette and 42 drifting light motes fade in, card pops in with a back-eased scale |
| 2 | `0.4 s` | **SYSTEM NOTICE** header, breathing halo behind the power symbol |
| 3 | `0.8 s` | `DISCONNECTED` title — each letter scrambles through random glyphs, then locks in |
| 4 | `1.5 s` | Subtitle typewriter: *"Gemini AI Assistant has been fully disabled."* |
| 5 | `2.6 s` | Divider grows from the centre, status rows slide in |
| 6 | `3.0 s` | Each subsystem scans amber, then locks to red **OFFLINE**: network bridge · Gemini API · local storage · code execution · input hooks |
| 7 | `4.6 s` | **Power cut** — the whole accent palette flips from indigo to red, the icon dips, the card shakes, RGB-split glitch on the title |
| 8 | `5.0 s` | Progress bar fills to 100 % with a live counter, then reads **SESSION TERMINATED** |
| 9 | `9.2 s` | The cinematic collapses; a pill badge fades in: `DISCONNECTED · gemini ai · offline` |
| 10 | idle | Comet chase around the mini power symbol, breathing glow, periodic shine sweep and glitch flicker |

The dot-ring power symbol, the comet chase, the dust field and every pulse are
driven by a **single `RenderStepped` loop**; tweens only handle the choreography.

### ⚙️ Configuration

All knobs live in the `CONFIG` table at the top of the file:

```lua
local CONFIG = {
    destroyLegacyGui  = true,   -- remove any leftover "GeminiAIGui" ScreenGui
    purgeLegacyData   = true,   -- delete "GeminiAI_Data.json" (plain-text API keys)
    keepBadge         = true,   -- stay on screen as a compact badge after the intro
    badgeBottomOffset = 96,     -- px from the bottom edge of the viewport
    introSpeed        = 1.0,    -- 1.0 = normal, 1.5 = faster, 0.5 = slower
    particles         = 42,     -- floating dust motes
    ringDots          = 26,     -- dots forming the power-symbol arc
    glitchy           = true,   -- occasional RGB-split glitch on the title
}
```

Set `keepBadge = false` and the overlay destroys itself right after the cinematic.

### 🖥️ Requirements

Nothing special — plain Roblox client API only (`Instance`, `TweenService`,
`RunService`, `UIScale`, `UIGradient`, `UIStroke`, `UICorner`). Executor
functions are used **only if they exist**: `gethui()` for a cleaner parent and
`delfile()` for the legacy key file. It also runs as an ordinary `LocalScript`.

---

## 🧾 Legacy Documentation

> ⚠️ Everything below this line describes the **old AI assistant**, which has
> been deleted from the script. It is kept for historical reference only —
> none of these features work anymore, and the installation snippets below
> will only show the DISCONNECTED overlay.

## ✨ Features

<table>
<tr>
<td width="50%">

### 🧠 Artificial Intelligence
- **23 Gemini models** - from lightweight to most powerful
- **Contextual memory** - AI remembers entire conversation
- **Smart responses** - help with code, advice, problem solving
- **Instant answers** - fast request processing

</td>
<td width="50%">

### 🎨 Interface
- **Modern design** - stylish and user-friendly UI
- **2 themes** - dark and light
- **Smooth animations** - pleasant experience
- **Drag & Drop button** - move it anywhere

</td>
</tr>
<tr>
<td width="50%">

### 💾 Functionality
- **Chat history** - save all conversations
- **Multiple API keys** - easy switching
- **Auto-save** - settings never lost
- **Copy text** - with one click

</td>
<td width="50%">

### 🌍 Localization
- **10 languages** - English, Russian, and more
- **Full translation** - entire interface
- **Quick switch** - in settings
- **Auto-save** - language remembered

</td>
</tr>
</table>

---

## 📥 Installation

### 🚀 Method 1: Loadstring (Recommended)

> ⚠️ **Legacy.** Running this today only plays the DISCONNECTED overlay — there is
> no assistant behind it anymore.

Copy and execute in any Roblox Executor:

```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/romokaso/Gemeni-AI/main/Gemeni-AI"))()
📋 Method 2: Manual Installation
Open the script file: Gemeni-AI
Click Raw button in top right corner
Copy all code (Ctrl+A → Ctrl+C)
Paste into your Executor
Click Execute/Inject
⚡ Method 3: With Error Handling
local success, err = pcall(function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/romokaso/Gemeni-AI/main/Gemeni-AI"))()
end)

if not success then
    warn("❌ Error loading Gemini AI:", err)
end
🔑 Getting API Key
⚠️ IMPORTANT: Without API key the script WILL NOT work! It's free and takes 2 minutes.
📝 Step-by-step guide:
�
🎯 Click to expand detailed instructions
Step 1: Open Google AI Studio
Go to: aistudio.google.com/apikey
Or copy in browser: https://aistudio.google.com/apikey
Step 2: Sign in
Click Sign in in top right corner
Sign in with your Google account
If you don't have an account - create one (free)
Step 3: Create API Key
Click blue button "Create API Key"
Select existing project or create new one
Wait a few seconds
Step 4: Copy the key
Your API key will appear (starts with AIza...)
Click Copy or select and copy manually
DON'T SHARE your key with others!
Step 5: Paste in script
Launch script in Roblox
Paste key in the window that appears
Click Confirm
Done! ✅
�

🎥 Video Tutorial
🎬 Video tutorial coming soon on YouTube
💡 Quick Link
Copy and open in browser:
https://aistudio.google.com/apikey
🎮 Usage
🎯 First Launch
Launch script via loadstring or manually
Enter API key in the window that appears
Click Confirm - key will be saved automatically
Button appears in top left corner of screen
Click the button to open chat
🖱️ Controls
Action
Description
Click button
Open/close interface
Drag
Move button to convenient place
📂 History
View all saved chats
⚙️ Settings
Change theme, language, API key
🤖 Model
Select Gemini model (23 options)
— Minimize
Minimize window
❌ Close
Close interface (return to key selection)
⌨️ Hotkeys
Enter in input field - send message
Copy button under message - copy to clipboard
▼ button bottom right - scroll down
💬 Usage Examples
👤 You: Write a teleport script for Roblox
🤖 AI: Sure! Here's an example teleport script...

👤 You: How to solve equation x² + 5x + 6 = 0?
🤖 AI: Let's solve this quadratic equation using discriminant...

👤 You: Translate "Hello World" to Japanese
🤖 AI: "Hello World" in Japanese is: こんにちは世界...

👤 You: Come up with a name for my space game
🤖 AI: Here are some ideas for a space game...
🤖 Available Models
�
📊 23 Gemini Models - click to expand
🏆 Pro Models (Most Powerful)
Best for complex tasks, programming, analysis
✨ Gemini 3 Pro - Newest top-tier model
🔬 Deep Research Pro - Deep analysis and research
💎 Gemini 2.5 Pro - Enhanced Pro version
🎯 Gemini Pro Latest - Latest stable Pro
⚡ Flash Models (Fast)
Balance of speed and quality for everyday tasks
🚀 Gemini 3 Flash - Newest fast model
⭐ Gemini 2.5 Flash - Enhanced Flash
🌟 Gemini 2.5 Flash Preview - Preview version 2.5
💫 Gemini 2.0 Flash - Stable 2.0
🔷 Gemini 2.0 Flash 001 - Specific 2.0 version
📌 Gemini Flash Latest - Latest stable Flash
🪶 Lite Models (Lightweight)
For simple questions, quick answers
🌙 Gemini 2.5 Flash Lite - Lightweight 2.5
⚪ Gemini 2.5 Flash Lite Preview - Lite 2.5 preview
🔹 Gemini 2.0 Flash Lite - Lightweight 2.0
💠 Gemini 2.0 Flash Lite 001 - Specific Lite 2.0
📍 Gemini Flash Lite Latest - Latest Lite
🧪 Experimental
Test and special models
🔬 Gemini Exp 1206 - Experimental (December 2024)
🍌 Nano Banana Pro - Specialized model
🎨 Gemma Models (Open Source)
Open models of different sizes
🦾 Gemma 3 27B - Largest (27 billion parameters)
💪 Gemma 3 12B - Medium (12 billion)
👍 Gemma 3 4B - Compact (4 billion)
🤏 Gemma 3 1B - Minimal (1 billion)
🔷 Gemma 3N E4B - Nano efficient 4B
🔹 Gemma 3N E2B - Nano efficient 2B
�

📊 Model Comparison
Model
Speed
Quality
Use Case
Pro
🐢 Slow
⭐⭐⭐⭐⭐
Complex tasks, code
Flash
⚡ Fast
⭐⭐⭐⭐
Daily conversations
Lite
🚀 Very fast
⭐⭐⭐
Simple questions
🌐 Supported Languages
Full interface translation in 10 languages:
�
￼
English
en ￼
Русский
ru ￼
Українська
uk ￼
Português
pt ￼
Indonesian
id ￼
日本語
ja ￼
Türkçe
tr ￼
العربية
ar ￼
Español
es ￼
Français
fr 
🔄 How to change language?
Open Settings (⚙️)
Click on current language
Select desired language from list
Language changes instantly!
⚙️ System Requirements
✅ Required Executor Functions
Your executor MUST support:
✔️ request() or http_request()  -- For API requests
✔️ readfile()                    -- Reading saved data
✔️ writefile()                   -- Saving settings
✔️ isfile()                      -- File checking
✔️ setclipboard()                -- Text copying
🎮 Compatible Executors
Tested and works on:
Executor
Status
Note
✅ Synapse X
Works
Full support
✅ Script-Ware
Works
Full support
✅ KRNL
Works
Full support
✅ Fluxus
Works
Full support
✅ Electron
Works
Full support
✅ Arceus X
Works
Full support
⚠️ JJSploit
Partial
Saving may not work
❌ Old executors
Doesn't work
No HTTP support
💻 Technical Specifications
📝 Language:          Lua 5.1
🔌 API:               Google Gemini Generative Language
🎨 UI:                Custom Roblox Instance
💾 Data format:       JSON
📦 Script size:       ~800 lines / ~50KB
🚀 RAM required:      Minimal
🔧 Troubleshooting
❌ Script doesn't start
�
Solution
Check executor - make sure it supports HTTP
Enable HttpService in game settings (if possible)
Try another executor from compatible list
Restart Roblox and try again
Check internet - active connection required
�

🔑 "Invalid API Key" / "API Error 400"
�
Solution
Check key:
Must start with AIza
Copied completely (usually 39 characters)
No spaces at start/end
Get new key:
Go to aistudio.google.com/apikey
Create new API key
Paste in script
Check limits:
New keys have limits (60 requests per minute)
Wait a few minutes if exceeded limit
�

⏱️ "Rate limit reached" / Error 429
�
Solution
What is this? You exceeded API request limit
Automatic solution:
Script will auto-switch to another model
Just wait for message
Manual solution:
Wait 1-2 minutes
Or add new API key in settings
Or switch to Lite model (fewer limits)
Gemini API Limits (free tier):
15 requests per minute (RPM)
1 million tokens per day
1500 requests per day
�

💾 Chat history doesn't save
�
Solution
Check executor functions:
print(writefile) -- Should output: function
print(readfile)  -- Should output: function
Write permissions:
Some executors require permissions
Check executor settings
Try another executor:
JJSploit often doesn't support saving
Use KRNL, Fluxus or others
Clear cache:
Delete GeminiAI_Data.json file (if exists)
Restart script
�

🖼️ Button doesn't appear
�
Solution
Wait for loading - may take 5-10 seconds
Check other corners - button might be off-screen
Restart script
Check console for errors (F9 in Roblox)
�

🌐 Language/theme doesn't change
�
Solution
This is normal! When changing language or theme:
GUI is completely recreated
You return to main screen
This is done for proper application of changes
Your data is saved:
Chat history ✅
API keys ✅
Selected model ✅
�

📱 Other Issues
�
Common problem solutions
Problem: AI responds in English instead of another language
Solution: Change language in settings affects only UI, not AI responses. For responses in your language, write in that language!
Problem: Takes long to respond/no response
Solution: Pro models think longer. Switch to Flash or Lite model
Problem: "Unexpected response format" error
Solution: Try another model, some experimental models are unstable
Problem: Script closes when clicking ❌
Solution: This is normal! ❌ closes GUI and returns to API key input. For minimize use —
�

💬 Need Help?
If problem not solved:
📝 Open Issue
📋 Describe problem in detail
📎 Attach error screenshot (if any)
💻 Specify your executor
📸 Screenshots
�

🌙 Dark Theme
Screenshots will be added later
☀️ Light Theme
Screenshots will be added later
⚙️ Settings
Screenshots will be added later
📂 Chat History
Screenshots will be added later
�

🤝 Contributing
Want to help improve Gemini AI? Any contribution is welcome!
🌟 How to help
�

🐛 Report a bug
Found a bug?
Open Issue
Describe problem
Attach screenshot
�

💡 Suggest feature
Have feature idea?
Open Issue
Describe feature
Explain why it's needed
�

🌍 Add translation
Know another language?
Fork repository
Add translation
Pull Request
�

📝 How to make Pull Request
Fork the repository
Click Fork button in top right corner
Clone your fork
git clone https://github.com/YOUR_USERNAME/Gemeni-AI.git
Create branch
git checkout -b feature/amazing-feature
Make changes and commit
git commit -m "Add amazing feature"
Push to your branch
git push origin feature/amazing-feature
Open Pull Request on GitHub
📜 Rules
✅ Follow project code style
✅ Test changes before PR
✅ Describe what changed and why
❌ Don't add malicious code
❌ Don't steal user API keys
📝 License
This project is licensed under MIT License - see LICENSE file
MIT License means you can:

✅ Use commercially
✅ Modify code
✅ Distribute
✅ Use privately
✅ Create forks

BUT you must:
⚠️ Include copy of license
⚠️ Credit original author
⚠️ Disclaimer
IMPORTANT! Read before using:
📚 This project created for educational purposes
⚖️ Author is not responsible for your use of script
⚠️ Author not responsible for Roblox bans
By using this script you agree to these terms!
👤 Author
�

romokaso
[
�
](https://github.com/romokaso)
[
�
](https://github.com/romokaso/Gemeni-AI)
Made with ❤️ for Roblox Community
�

🌟 Support the Project
If project helped you or you liked it:
�

⭐ Star the repo - helps others find project
🔄 Fork it - create your own version
📢 Tell friends - share the link
💬 Leave feedback - write what you think
[
�
](https://github.com/romokaso/Gemeni-AI)
[
�
](https://github.com/romokaso/Gemeni-AI/fork)
[
�
](https://github.com/romokaso/Gemeni-AI)
�

📊 Statistics
�

�
�
�
�
�
�
�

📞 Contact
Have questions? Contact me:
📧 GitHub Issues: Create Issue
💬 Discussions: Discussions
🐛 Bug Reports: Report Bug
📈 Changelog
�
Version History
v1.0.0 (February 17, 2025)
✨ First public release
🧠 Support for 23 Gemini models
🌍 10 interface languages
💾 Chat history system
🔑 Multiple API key management
🎨 Dark and light theme
🖱️ Drag & Drop button
💾 Auto-save settings
📋 Message copying
�

�

�
🎉 Thank you for using Gemini AI!
Made with ❤️ for Roblox Community
⬆ Back to top
�
�
```
