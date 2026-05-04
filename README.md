# Deutsch Lernen mit Talha

Interactive German A1 exercise app. Upload any German lecture PDF and Gemini automatically extracts and converts every exercise into an interactive practice session.

## Features

- **Upload any German PDF** — Gemini reads it directly and extracts exercises
- **4 exercise types** auto-classified: Writing, Speaking, Listening, Reading
- **Writing**: Type answers, get instant AI feedback
- **Speaking**: Record your voice, get strict pronunciation evaluation, hear the corrected version spoken back to you by Gemini TTS
- **Listening**: YouTube links auto-embedded, comprehension questions checked by AI
- **Reading**: Read passage, answer questions, AI grades comprehension
- **TTS caching**: Audio cached after first play for instant replay

## Setup

1. Open the live site (or `index.html` locally in Chrome/Edge)
2. Get a free [Gemini API key](https://aistudio.google.com/app/apikey)
3. Paste it in the yellow bar at the top and click Save
4. Upload a PDF and start practicing

## Tech

- Pure HTML/CSS/JS — no build step
- Gemini 3 Flash Preview for evaluation + audio understanding
- Gemini 2.5 Flash Preview TTS for German pronunciation
- MediaRecorder API for voice capture

## Local development

Just open `index.html` in a modern browser. Microphone access requires Chrome or Edge.
