# Deutsch Lernen

Interactive German A1 exercise app. Upload any German lecture PDF and Gemini automatically extracts and converts every exercise into an interactive practice session.

## Features

- **Upload any German PDF** — Gemini reads it directly and extracts exercises
- **2 exercise types** auto-classified: Writing, Speaking
- **Writing**: Type answers, get instant AI feedback
- **Speaking**: Record your voice, get strict pronunciation evaluation, hear the corrected version spoken back to you by Gemini TTS
- **TTS caching**: Audio cached after first play for instant replay

## Setup

1. Open the live site (or `index.html` locally in Chrome/Edge)
2. **Get a free Gemini API key** — see step-by-step below
3. Paste it in the yellow bar at the top and click **Save**
4. Upload a PDF and start practicing

## How to get a free Gemini API key (beginner guide)

Gemini gives you a generous free tier — perfect for this app. No credit card needed.

### Step 1 — Open Google AI Studio
Go to **https://aistudio.google.com/app/apikey** in your browser.

### Step 2 — Sign in with a Google account
- Click **Sign in** (top-right)
- Use any Gmail / Google account
- Accept the Terms of Service when prompted

### Step 3 — Create the API key
- You'll land on the **API keys** page
- Click the blue **Create API key** button
- A popup asks you to pick a Google Cloud project — just click **Create API key in new project** (it makes one automatically)
- Wait 5–10 seconds while Google generates it

### Step 4 — Copy the key
- The key looks like `AIzaSy…` (about 40 characters long)
- Click the **copy icon** next to it
- ⚠️ Keep this key private — anyone with it can use your free quota

### Step 5 — Paste it into the app
- Open the app (live site or local `index.html`)
- Paste the key into the **yellow bar at the top** that says *"Enter your Gemini API key…"*
- Click **Save**
- It's stored only in your browser's local storage — nothing is sent to any server other than Google

### Step 6 — Start using it
Upload a PDF and the app will use your key to call Gemini for:
- Reading & extracting exercises from the PDF
- Grading your written answers
- Listening to your spoken answers and judging pronunciation
- Speaking corrected German pronunciation back to you (TTS)

### Free tier limits (more than enough for personal study)
- ~1,500 requests/day on Gemini Flash models
- 15 requests/minute
- If you ever hit a limit, just wait a minute and try again — the key still works

### Troubleshooting

- **"API Error: ... not found for API version v1beta"** → The model name in the code is wrong, or your account region doesn't have access yet. Try refreshing the page.
- **"API Error: 400"** → Usually the key was pasted with a stray space. Re-copy and re-paste.
- **"API Error: 403"** → The key is invalid or the Generative Language API isn't enabled. Go back to AI Studio and recreate the key.

## Tech

- Pure HTML/CSS/JS — no build step
- Gemini 3 Flash Preview for evaluation + audio understanding
- Gemini 2.5 Flash Preview TTS for German pronunciation
- MediaRecorder API for voice capture

## Local development

Just open `index.html` in a modern browser. Microphone access requires Chrome or Edge.
