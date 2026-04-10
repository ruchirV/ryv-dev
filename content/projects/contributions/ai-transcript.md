---
title: "AI Transcript"
date: 2026-01-01
featured: true
description: "AI-powered voice transcription with Whisper and LLM cleaning. Browser-based recording interface with FastAPI backend."
tags: ["OpenAI", "LLM", "Speech-To-Text", "React", "Python","Typescript"]
link: "https://github.com/ruchirV/local-ai-transcript-app"
weight: 200
type: "projects"
---

The AI Transcript App is a full-stack tool that records your voice, transcribes it locally using Whisper, and cleans the resulting text with an LLM — removing filler words, fixing grammar, and preserving meaning.

It's designed to run entirely on your machine with no cloud dependency, though it supports any OpenAI-compatible cloud API as a drop-in replacement.

---

- This is a study project forked from [AI-Engineer-Skool](https://www.skool.com/ai-engineer)

---

**Features:**

- Browser-based voice recording (hold *V* to record)
- Audio file upload via drag-and-drop
- Whisper speech-to-text (runs locally via *faster-whisper*)
- LLM-powered transcript cleaning (removes filler words, fixes errors)
- Manual text input — paste any text for LLM cleaning
- Customizable LLM system prompt
- One-click copy to clipboard
- OpenAI API-compatible — works with Ollama, LM Studio, OpenAI, or any compatible provider

---

**Stack:**

| Layer | Technology |
|-------|-----------|
| Frontend | React 19, TypeScript, Vite |
| Backend | FastAPI, Python 3.12, uv |
| Speech-to-Text | faster-whisper (local) |
| LLM | OpenAI Python SDK → Ollama (default) |
| Containerization | Docker Compose |

---
