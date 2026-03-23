# SquadOps AI Setup Guide
### Your AI Business Assistant — Ready in 12 Minutes

---

## Before You Start

You'll need:
- ✅ **12 minutes** of uninterrupted time
- ✅ **Your phone** (for Telegram setup)
- ✅ **Basic business info** (services, hours, etc.)

---

## Step 1: Download the Installer

After purchase, download the installer for your computer:

| Your Computer | Download |
|---------------|----------|
| **Mac (M1/M2/M3/M4)** | squadops-setup-macos-arm64 |
| **Mac (Intel)** | squadops-setup-macos-x64 |
| **Windows** | squadops-setup-win-x64.exe |
| **Linux** | squadops-setup-linux-x64 |

**Not sure which Mac you have?**
→ Click the Apple logo → "About This Mac"
→ If it says "Apple M1/M2/M3/M4" = Apple Silicon
→ If it says "Intel" = Intel

---

## Step 2: Run the Installer

### On Mac

1. Open **Finder**
2. Go to your **Downloads** folder
3. Find `squadops-setup-macos-arm64` (or the x64 version)
4. **Right-click** it → **Open**
5. Click **Open** again if you see a security warning
6. A Terminal window will open — this is normal!

**Can't open it?**
→ Go to System Settings → Privacy & Security
→ Scroll down and click "Open Anyway" next to the SquadOps message

### On Windows

1. Open **File Explorer**
2. Go to your **Downloads** folder
3. Double-click `squadops-setup-win-x64.exe`
4. Click **Run Anyway** if SmartScreen appears
5. A Command Prompt window will open — this is normal!

**SmartScreen blocking it?**
→ Click "More info" → "Run anyway"

### On Linux

1. Open **Terminal**
2. Navigate to Downloads: `cd ~/Downloads`
3. Make it executable: `chmod +x squadops-setup-linux-x64`
4. Run it: `./squadops-setup-linux-x64`

---

## Step 3: Install Node.js (If Needed)

If you see this message:

```
⚠️ Node.js Required
```

Don't worry! Just:

1. **Click "Y"** to open nodejs.org in your browser
2. Click the green **"LTS"** button (left side)
3. Run the downloaded installer
4. Click through (Next → Agree → Install)
5. **Close your terminal** and start the SquadOps installer again

---

## Step 4: Answer the Setup Questions

The installer will ask you about your business. Answer honestly — this teaches your AI assistant how to represent you!

### Basic Info (2 min)
- Your industry
- Business name
- Your name
- Phone number

### Business Profile (3 min)
- What services you offer
- Your service area
- Business hours
- Your pricing approach

### How You Work (5 min)
- Your business story
- What makes you different
- Common customer objections (and how you handle them)
- Your availability preferences
- What counts as an emergency

### Technical Setup (2 min)
- Set up Telegram (see Step 5)
- Choose your AI provider (xAI recommended)

---

## Step 5: Set Up Telegram

Telegram is how you'll communicate with your AI assistant. Here's exactly how to set it up:

### A. Create a Telegram Account (if you don't have one)

1. Download Telegram on your phone:
   - iPhone: [App Store](https://apps.apple.com/app/telegram-messenger/id686449807)
   - Android: [Play Store](https://play.google.com/store/apps/details?id=org.telegram.messenger)
2. Open Telegram and sign up with your phone number

### B. Create Your Bot

1. Open Telegram
2. Search for **@BotFather** (it has a blue checkmark)
3. Tap **Start**
4. Type: `/newbot`
5. Enter a name for your bot (e.g., "Hansen Plumbing Assistant")
6. Enter a username ending in `bot` (e.g., "HansenPlumbingBot")
7. **Copy the token** BotFather gives you (looks like: `123456789:ABCdef...`)
8. Paste this token in the installer when asked

### C. Get Your User ID

1. In Telegram, search for **@userinfobot**
2. Tap **Start**
3. It will show your User ID (a number like `123456789`)
4. Enter this in the installer when asked

---

## Step 6: Get Your xAI API Key

xAI powers your AI assistant. Here's how to get a key:

1. Go to [console.x.ai](https://console.x.ai)
2. Sign up or log in
3. Click **"Create API Key"**
4. Copy the key (starts with `xai-...`)
5. Paste it in the installer when asked

**Cost:** About $0.10-0.50 per day depending on usage. Very affordable!

---

## Step 7: Complete Setup

1. Answer any remaining questions
2. Wait for installation to complete
3. When you see "🎉 Your AI Assistant is Ready!" — you're done!

---

## Step 8: Test Your Assistant

1. Open **Telegram**
2. Search for your bot's username
3. Tap **Start**
4. Send: `Hi!`
5. Your assistant should respond!

### Try These Messages

- "What can you do?"
- "Tell me about my business"
- "Help me respond to a customer who wants a quote"
- "What are my business hours?"

---

## Troubleshooting

### "Node.js not found"
→ Install Node.js from [nodejs.org](https://nodejs.org)
→ Close your terminal and run the installer again

### "Permission denied" on Mac
→ Run: `sudo npm install -g openclaw@latest`
→ Enter your Mac password when asked

### "Permission denied" on Windows
→ Right-click Command Prompt → "Run as Administrator"
→ Run the installer again

### Bot doesn't respond
1. Make sure the installer finished completely
2. Check that OpenClaw is running:
   - Mac/Linux: `openclaw status`
   - Windows: Open a new Command Prompt and type `openclaw status`
3. Restart if needed: `openclaw gateway restart`

### Can't find my Telegram User ID
→ Search for @userinfobot in Telegram
→ Send it any message
→ It will reply with your ID

### I made a mistake during setup
No problem! Just run the installer again. Your answers are saved, and you can update them.

---

## Daily Usage Tips

### Keep Terminal Open
Your AI assistant runs in your Terminal/Command Prompt. Keep this window open (you can minimize it).

### Auto-Start (Recommended)
During setup, say **Yes** to "Start automatically?" — this way your assistant runs even after you restart your computer.

### Check on Your Assistant
- `openclaw status` — See if it's running
- `openclaw gateway restart` — Restart if needed

---

## Getting Help

**Email:** support@squadops.xyz

When contacting support, please include:
- Your computer type (Mac/Windows/Linux)
- What step you're stuck on
- Any error messages you see

We typically respond within 24 hours!

---

## What's Next?

Your AI assistant is now ready to:
- ✅ Respond to customer inquiries
- ✅ Schedule appointments
- ✅ Follow up with leads
- ✅ Answer common questions
- ✅ Handle after-hours messages

**The more you use it, the smarter it gets!**

Start forwarding customer messages to your bot, or give customers your bot's Telegram link directly.

---

*Welcome to SquadOps AI! 🎉*
