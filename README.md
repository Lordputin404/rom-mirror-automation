🚀 ROM Mirror Automation (Multi-Host → SourceForge)

A fully automated GitHub Actions workflow to mirror ROM builds from multiple sources (Google Drive, direct links, etc.) to SourceForge — with zero manual effort.

---

✨ Features

- 🔄 One-click mirror via GitHub Actions
- 🌐 Supports:
  - Google Drive links
  - Direct download links
- 📁 Dynamic SourceForge folder selection
- 📛 Preserves original filename
- ⚡ No local upload required
- 🤖 Fully automated pipeline
- 📲 Telegram notifications (start, success, failure)

---

🧠 How It Works

This workflow performs the following steps:

1. 📥 Downloads the file from the provided link
2. 🏷 Automatically detects the filename
3. 📤 Uploads it to SourceForge via SFTP
4. 📲 Sends status updates to Telegram

---

⚙️ Setup Guide

1️⃣ Add GitHub Secrets

Go to your repository → Settings → Secrets → Actions

Add the following:

🔐 SourceForge

- "SF_USER" → Your SourceForge username
- "SF_PASSWORD" → Your SourceForge password
- "SF_PROJECT" → Your SourceForge project name

📲 Telegram (Optional but Recommended)

- "TG_BOT_TOKEN" → Your Telegram bot token
- "TG_CHAT_ID" → Your Telegram chat ID

---

🤖 Telegram Setup

1. Open Telegram and search for BotFather
2. Create a new bot using "/newbot"
3. Copy the bot token

To get your chat ID:

- Use a bot like "userinfobot"
- Start it and copy your ID

---

🚀 Usage

1. Go to Actions tab in your repository
2. Select ROM Mirror workflow
3. Click Run workflow
4. Enter:
   - "file_url" → Google Drive or direct download link
   - "sf_folder" → Target folder name on SourceForge

---

📦 Example

Input| Value
File URL| Google Drive / Mirror link
Folder| Lunaris-AOSP

➡️ Output: File uploaded to SourceForge automatically

---

⚠️ Notes

- Minimum file size validation prevents broken downloads
- Resume supported for large files
- Works best for ".zip" ROM packages (but supports other formats)

---

🔮 Future Improvements

- Multi-file support
- Upload progress tracking
- Retry system for failed uploads
- Telegram command-based triggers
- Web UI panel

---

❤️ Contribution

Contributions are welcome!
Feel free to fork and improve this project.

---

📜 License

Open-source — free to use and modify.
