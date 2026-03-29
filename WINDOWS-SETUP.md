# SquadOps AI — Windows Setup Guide

## Quick Start (5 minutes)

### Step 1: Download the Installer
1. Go to: https://github.com/jrbobbyhansen-pixel/squadops-releases/releases/latest
2. Download `squadops-setup-win-x64.exe`
3. Right-click the file → "Run as administrator" (if prompted about security, click "More info" → "Run anyway")

### Step 2: Run the Setup
The installer will guide you through:
1. **License validation** — enter the email you used to purchase
2. **Business info** — your business name and industry
3. **Productivity suite** — choose Google Workspace or Microsoft 365
4. **Telegram bot creation** — follow the BotFather prompts

### Step 3: Connect Your Services

**If you chose Google Workspace:**
```
gog auth add youremail@gmail.com
```
Then follow the browser prompt to authorize.

**If you chose Microsoft 365:**
Your Outlook integration works automatically with your desktop Outlook app.

### Step 4: Start Chatting!
Open Telegram, find your new bot, and send a message. Your AI assistant is ready.

---

## What Works on Windows

✅ **Full AI Chat** — Your assistant responds to any question  
✅ **Google Workspace** — Gmail, Calendar, Drive, Contacts  
✅ **Microsoft Outlook** — Read and send emails via your desktop Outlook  
✅ **Web Search** — Research anything online  
✅ **Weather** — Get forecasts for any location  
✅ **Humanizer** — All outbound messages sound natural  
✅ **PDF Generation** — Create quotes, contracts, documents  
✅ **YouTube/Article Summaries** — Summarize any content  
✅ **Obsidian Notes** — Cross-platform markdown notes  

---

## Troubleshooting

### "Node.js not found"
1. Download Node.js from https://nodejs.org (click the green LTS button)
2. Run the installer
3. **Restart your terminal/command prompt**
4. Run the SquadOps setup again

### Bot not responding
Run these commands:
```
openclaw gateway status
openclaw gateway restart
```

### Need help?
Email: bobby@squadops.xyz

---

## What's Different from Mac

| Feature | Mac | Windows |
|---------|-----|---------|
| Calendar | Apple Calendar OR Google | Google OR Outlook |
| Reminders | Apple Reminders OR Google Tasks | Google Tasks OR Outlook Tasks |
| Notes | Apple Notes OR Obsidian | Obsidian OR OneNote |
| Text messaging | iMessage | WhatsApp (optional) |
| Email | Apple Mail OR Gmail | Gmail OR Outlook |

The core AI assistant works identically — you just connect different services.
