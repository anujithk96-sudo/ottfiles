# Deploying to Railway (Free Hosting)

Railway gives you free hosting for bots — no credit card needed for basic use.

## Step 1 — Push bot to GitHub

Create a new GitHub repo called `ott-telegram-bot` and push these files:

```bash
git init
git add .
git commit -m "Initial commit: OTT Telegram bot"
git remote add origin https://github.com/YOUR_USERNAME/ott-telegram-bot.git
git push -u origin main
```

## Step 2 — Sign up on Railway

1. Go to **railway.app**
2. Click **Login with GitHub**
3. Authorise Railway

## Step 3 — Create a new project

1. Click **New Project**
2. Choose **Deploy from GitHub repo**
3. Select your `ott-telegram-bot` repo
4. Railway auto-detects Python and installs requirements

## Step 4 — Add environment variables

1. Click your project → **Variables** tab
2. Add:
   - `TELEGRAM_BOT_TOKEN` = your token from BotFather
   - `ALLOWED_USER_IDS`   = your Telegram user ID

## Step 5 — Deploy

1. Click **Deploy**
2. Watch the build logs — it should say `Bot is running...`
3. Your bot is now live 24/7!

## Checking logs

Railway → your project → **Deployments** → click latest → **View Logs**

## Free tier limits

Railway free tier gives $5 credit/month which is enough to run a lightweight
bot 24/7. No downloads are stored on Railway — they go to your output/ folder
on the server or you can configure an external storage path.
