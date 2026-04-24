# TwinMind Live Suggestions Copilot

Live demo: https://fascinating-tartufo-4735c0.netlify.app

## Setup
1. Open the deployed URL in Chrome
2. Click Settings, paste your Groq API key
3. Click Start and begin talking

## Stack
- Vanilla HTML, CSS, JavaScript — single file
- Groq Whisper Large V3 for transcription
- Llama 3.3 70B Versatile for suggestions and chat
- Netlify for hosting

## Prompt Decisions
- 4000 char context window for suggestions = ~2-3 mins of speech
- 3 suggestions forced to be different types each refresh
- Preview text delivers value without clicking
- 12000 char context for chat = full session memory
- 30s refresh interval balances speed vs cost

## Tradeoffs
- Single HTML file for simplicity and zero build complexity
- localStorage persists API key across sessions
- Client side only, no backend, no data stored anywhere
