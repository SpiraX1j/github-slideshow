# JARVIS

A voice-controlled personal AI assistant that runs entirely in your browser, with Claude as its brain.

## Run it
- **Locally:** open `jarvis/index.html` in Chrome or Edge (they support voice input). Or run `python3 -m http.server` from the repo root and visit `http://localhost:8000/jarvis/`.
- **GitHub Pages:** once Pages is enabled for this repo, it's served at `/jarvis/`.

Open **Settings**, paste your Anthropic API key (from console.anthropic.com), and talk.

## What it does
- **Voice in and out:** click the core or press Space to talk. Replies are spoken sentence by sentence as they stream in. Esc stops speech.
- **Wake word (optional):** turn on "Always listen" in Settings, then say "Jarvis, …".
- **Instant local commands (no API key needed):** "what time is it", "what's the date", "open youtube" / "open example.com", "search for …", "set a timer for 5 minutes", "stop", "clear memory".
- **Everything else goes to Claude** (`claude-opus-5-5`, low effort for snappy replies), with conversation memory and optional web search for live info like news and weather.

## Privacy
Your API key is stored only in this browser's localStorage and sent only to `api.anthropic.com`. Don't use it on a shared computer.
