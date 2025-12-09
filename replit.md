
# Baka-Chan Messenger Bot (Goat-Bot-business)

## Overview
A Facebook Messenger chatbot based on Goat-Bot-business framework, merged with custom commands from baka-chan-v1. The bot uses unofficial Facebook Chat API (fca-gtajisan) for connecting to Messenger.

## Developer
- **Name**: Gtajisan (Farhan)
- **Email**: ffjisan804@gmail.com
- **GitHub**: https://github.com/Gtajisan

## Project Structure
```
/
├── bot/                    # Core bot logic
│   ├── handler/           # Message and event handlers
│   └── login/             # Login and authentication
├── dashboard/             # Web dashboard for bot management
├── database/              # SQLite database files
├── func/                  # Utility functions
├── languages/             # Language files (en, vi)
├── logger/                # Logging utilities
├── neokex_fca_database/   # Custom FCA (Facebook Chat API) by Gtajisan
├── scripts/
│   ├── cmds/              # Bot commands (156+ commands)
│   └── events/            # Event handlers (welcome, leave, etc.)
├── account.txt            # Facebook cookies (DO NOT SHARE)
├── config.json            # Main bot configuration
├── configCommands.json    # Command settings
├── index.js               # Entry point
└── Goat.js                # Main bot file
```

## Configuration

### config.json
- `prefix`: Command prefix (default: "!")
- `adminBot`: Array of admin Facebook UIDs
- `nickNameBot`: Bot display name
- `language`: Bot language (en/vi)
- `database.type`: Database type (sqlite/mongodb/json)
- `publicInboxMode`: Enable public inbox mode for business accounts

### account.txt
Contains Facebook cookies in JSON format. Required for authentication.

## Commands
The bot has 150+ commands including:
- **AI**: ai, gpt, metaai, midjourney
- **Media**: video, sing, pinterest, anime
- **Utility**: help, admin, prefix, uid
- **Fun**: quiz, rank, daily, meme
- **Moderation**: ban, kick, warn, whitelist

Use `!help` to see all available commands.

## Running the Bot
The bot runs via the "Goatbot Messenger" workflow:
```bash
node index.js
```

Dashboard available at port 3001.

## Credits
- Original Goat-Bot-V2 by NTKhang (https://github.com/ntkhang03)
- Business Version & Enhanced by Gtajisan (https://github.com/Gtajisan)
- Developer: Gtajisan (Farhan) - ffjisan804@gmail.com

## Recent Changes
- 2025-12-09: Merged baka-chan-v1 commands with Goat-Bot-business base
- Configured for business account inbox with public access
- Fixed duplicate command conflicts
- Removed broken/incompatible commands
- Rebranded from neokex to Gtajisan
