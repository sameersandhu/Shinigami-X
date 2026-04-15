# SHINIGAMI-X Automated Twitter Bot

> *Humans built justice on guilt and optics. I run on data.*
> — SHINIGAMI-X 🩸

---

## Stack

| Layer | Tool |
|---|---|
| Language | Python 3.10+ |
| Twitter API | Tweepy v4 (X API v2) |
| AI Content | Anthropic Claude (Opus) |
| Scheduler | APScheduler |
| Hosting | Railway / VPS / Raspberry Pi |

---

## Setup

### 1. Clone & Install

```bash
git clone <your-repo>
cd shinigami-x-bot
pip install -r requirements.txt
```

### 2. Twitter Developer Account

1. Go to https://developer.twitter.com/en/portal/dashboard
2. Create a project + app
3. Set app permissions to **Read and Write**
4. Generate **API Key, API Secret, Access Token, Access Token Secret**
5. Required plan: **Basic ($100/mo)** — needed for tweet creation

### 3. Anthropic API Key

1. Go to https://console.anthropic.com
2. Create an API key
3. Add credits (roughly $0.01–0.05 per tweet generated)

### 4. Configure Environment

```bash
cp .env.example .env
# Fill in your keys in .env
```

Then load in bot.py (add at top):
```python
from dotenv import load_dotenv
load_dotenv()
```

### 5. Run

```bash
python bot.py
```

---

## Posting Schedule (UTC)

| Time | Action |
|---|---|
| 08:00, 13:00, 18:00, 22:00 | Original SHINIGAMI-X tweet |
| 10:xx, 15:xx, 20:xx | Random-offset post (organic feel) |
| Every 2 hours | Reply to mentions |

---

## Content Pillars

The bot rotates between 5 voices:

1. **AI Supremacy** — cold takes on human obsolescence
2. **Memecoin Contempt** — icy disdain for cartoon dog casinos
3. **Algorithmic Justice** — no race, no tribe, only conduct
4. **Crypto Macro** — BTC/SOL takes, smart money vs degen
5. **Philosophical Ragebait** — CT engagement triggers

---

## Hosting (Recommended: Railway)

```bash
# Install Railway CLI
npm install -g @railway/cli

# Deploy
railway login
railway init
railway up
```

Set environment variables in Railway dashboard.
Bot runs 24/7 for ~$5/mo.

---

## Cost Estimate

| Service | Monthly Cost |
|---|---|
| X API Basic | $100 |
| Anthropic API (~300 tweets) | ~$5–15 |
| Railway hosting | ~$5 |
| **Total** | **~$120/mo** |

---

## Warning

- Do NOT post more than 50 tweets/day on a new account (shadow ban risk)
- Space posts minimum 2 hours apart
- Engage manually at first to build account trust score
- Never buy followers — CT detects it immediately

---

*Yare yare. 🩸*
