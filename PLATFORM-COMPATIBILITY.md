# SquadOps Installer — Platform Compatibility Matrix

## Supported Platforms

| Platform | Architecture | Binary | Status |
|----------|--------------|--------|--------|
| macOS | ARM64 (M1/M2/M3/M4) | squadops-setup-macos-arm64 | ✅ Full |
| macOS | x64 (Intel) | squadops-setup-macos-x64 | ✅ Full |
| Windows | x64 | squadops-setup-win-x64.exe | ✅ Full |
| Windows | ARM64 | squadops-setup-win-x64.exe* | ⚠️ Via Emulation |
| Linux | x64 | squadops-setup-linux-x64 | ✅ Full |
| Linux | ARM64 | squadops-setup-linux-x64* | ❌ Not Built |

*Windows ARM64 runs x64 binary via emulation. Linux ARM64 would need separate build.

---

## Feature Matrix by Platform

### Productivity Integration

| Feature | macOS | Windows | Linux |
|---------|-------|---------|-------|
| Google Workspace (gog) | ✅ Homebrew | ✅ GitHub download | ✅ GitHub download |
| Apple iCloud | ✅ Native | ❌ N/A | ❌ N/A |
| Microsoft Outlook | ✅ Graph API | ✅ COM automation | ✅ Graph API |
| Obsidian Notes | ✅ | ✅ | ✅ |

### Universal Skills (All Platforms)

| Skill | Description | Platform Notes |
|-------|-------------|----------------|
| gog | Google Workspace | ARM64 supported on all platforms |
| humanizer | AI text humanization | Pure skill, no binary |
| weather | Weather lookups | Pure skill, no binary |
| obsidian | Markdown notes | Pure skill, no binary |
| summarize | Content summarization | OpenClaw skill, no binary |

### Platform-Specific Skills

| Skill | macOS | Windows | Linux |
|-------|-------|---------|-------|
| apple-reminders | ✅ | ❌ | ❌ |
| apple-calendar | ✅ | ❌ | ❌ |
| apple-notes | ✅ | ❌ | ❌ |
| imsg | ✅ | ❌ | ❌ |
| ms-outlook-teams-assistant | ❌ | ✅ (COM) | ❌ |
| outlook-delegate | ✅ | ✅ | ✅ |

---

## Installation Paths

### Node.js Detection
- **macOS**: `/usr/local/bin/node`, `/opt/homebrew/bin/node`, `~/.nvm/`
- **Windows**: `C:\Program Files\nodejs\`, `%APPDATA%\npm\`, `where node`
- **Linux**: `/usr/local/bin/node`, `/usr/bin/node`, `~/.nvm/`

### gog CLI Installation
- **macOS**: `brew install steipete/tap/gogcli`
- **Windows**: PowerShell download from GitHub releases → `~/.squadops/bin/gog.exe`
- **Linux**: curl download from GitHub releases → `~/.squadops/bin/gog`

### gog Token Storage
- **macOS**: `~/Library/Application Support/gogcli/credentials.json`
- **Windows**: `%APPDATA%\gogcli\credentials.json`
- **Linux**: `~/.config/gogcli/credentials.json`

### OpenClaw Workspace
- **All platforms**: `~/.openclaw/` (default) or `~/squadops-workspace/` (legacy)

---

## Error Handling

### npm Permission Errors
- **macOS/Linux**: Automatically retries with `sudo`
- **Windows**: Prompts user to run as Administrator

### Binary Download Failures
- **All platforms**: Falls back gracefully, skill works without native binary

### Network Timeouts
- **All platforms**: 60-second timeout on downloads, graceful fallback

---

## Known Limitations

1. **Windows ARM64**: Must use x64 binary via emulation (no native ARM64 build)
2. **Linux ARM64**: Not currently built (would need pkg build target addition)
3. **Google OAuth**: Requires correctly configured redirect URI in Google Cloud Console
4. **Apple Skills**: Only work on macOS (AppleScript dependency)
5. **MS Outlook COM**: Only works on Windows with Outlook desktop installed

---

## Testing Checklist

Before release, verify on each platform:

- [ ] Binary executes without crash
- [ ] Node.js detection works
- [ ] npm install openclaw succeeds
- [ ] Productivity selection shows correct options
- [ ] gog binary downloads (if Google selected)
- [ ] Gateway installs and starts
- [ ] Bot responds in Telegram
- [ ] OAuth flow completes (if Google selected)

---

*Last updated: 2026-03-29*
