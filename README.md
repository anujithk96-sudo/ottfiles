# 🤖 OTT Downloader Telegram Bot

A Telegram bot that lets you trigger OTT downloads directly from your phone.

## Commands

| Command | Description |
|---|---|
| `/start` | Welcome message |
| `/rip <platform> <url> [quality]` | Start a download |
| `/status` | View active downloads |
| `/cancel <job_id>` | Cancel a download |
| `/platforms` | List all 20+ supported platforms |
| `/help` | Full help |

## Examples

```
/rip jiocinema https://www.jiocinema.com/... 4K
/rip netflix https://www.netflix.com/watch/... 1080p shows
/rip aha https://www.aha.video/... 720p movies
```

## Setup

### Step 1 — Create your bot on Telegram
1. Open Telegram → search **@BotFather**
2. Send `/newbot`
3. Give it a name e.g. `OTT Downloader`
4. Give it a username e.g. `myott_downloader_bot`
5. Copy the **token** it gives you

### Step 2 — Get your Telegram user ID
1. Open Telegram → search **@userinfobot**
2. Send `/start`
3. Copy your **ID number**

### Step 3 — Configure .env
```bash
cp .env.example .env
# Edit .env and paste your token and user ID
```

### Step 4 — Install dependencies
```bash
pip install -r requirements.txt
```

### Step 5 — Run locally
```bash
python bot.py
```

### Step 6 — Deploy to Railway (free)
See DEPLOY.md for full instructions.
