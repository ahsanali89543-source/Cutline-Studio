# Cutline Studio

Video captioning and editing studio with Roman Urdu support, pro timeline, WebCodecs MP4 export, and more.

## Features

- **Transcription** for Roman Urdu (xAI Grok STT / Groq / OpenAI Whisper + romanization)
- **Pro timeline** with captions / video filmstrip / audio waveform tracks
- **MP4 export** with WebCodecs (H.264 + AAC), captions burned in
- **47 caption templates** + motion presets
- Landing site with features, pricing (launch free), FAQ

## Getting started

```bash
npm install
npm run dev
```

See `CUTLINE-UPDATE.md` for recent changes and environment variables.

## Environment variables

| Variable | Needed? | Purpose |
|---|---|---|
| `XAI_API_KEY` | Injected by the Grok platform | Grok Voice transcription + Roman Urdu AI pass |
| `GROQ_API_KEY` | Optional backup | Whisper large-v3 transcription + romanizer |
| `OPENAI_API_KEY` | Optional backup | Whisper + romanizer |
| `TRANSCRIBE_PROVIDERS` | Optional | Order, e.g. `groq,xai` |
| `LEADS_WEBHOOK_URL` | Optional | Creator sign-ups forwarded here |

## Original upload

This repository was created from the `Cutline-Studio.zip` project archive.
Some large media assets (hero images, etc.) may need to be added separately if not present.
