# YouTube Shorts Automation Service

This package contains a practical n8n-oriented automation design for generating and publishing YouTube Shorts using a stock + text format.

## Goal
Automate a daily Shorts pipeline for clients as a service:
- topic selection
- script generation
- voiceover text generation
- stock visual plan
- metadata generation
- YouTube upload

## Recommended stack
- n8n
- OpenAI
- ElevenLabs or OpenAI TTS
- FFmpeg
- Pexels or Pixabay API
- YouTube Data API

## Flow summary
1. Daily trigger
2. Load client brief
3. Generate topic + hook + 60s script
4. Generate title, description, hashtags
5. Generate voiceover text
6. Generate stock shot list
7. Fetch stock assets
8. Render subtitle-based Shorts video
9. Upload to YouTube Shorts
10. Log result

## Notes
This repo package includes:
- workflow.json
- client-brief.json
- prompt-pack.json
- render-spec.json

Some nodes require credentials and custom adaptation in n8n.
