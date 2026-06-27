# Arabic Voice Assistant - Dental Clinic Receptionist

An intelligent Arabic voice assistant for a dental clinic reception, built with Streamlit, Vosk for speech recognition, and OpenRouter for AI-powered conversations.

## Overview

This application is a complete voice-enabled receptionist system for "Vancouver Dental Clinic" that allows patients to interact naturally using Arabic voice or text. The assistant handles appointment scheduling, clinic information queries, and general inquiries about dental services.

## Features

- Arabic speech recognition using Vosk
- Natural language understanding via OpenRouter (Gemma-2-9b-it)
- Text-to-speech output using gTTS
- Multiple interaction modes: Text, Voice, or Combined (Twins)
- Auto-recording after responses
- Voice input via microphone or file upload
- Professional dental clinic context with predefined system prompt
- Session history with audio playback
- Microphone testing tool

## Technologies

| Component | Technology |
|-----------|-----------|
| STT (Speech-to-Text) | Vosk (Arabic model) |
| LLM | OpenRouter (google/gemma-2-9b-it) |
| TTS (Text-to-Speech) | gTTS |
| UI Framework | Streamlit |
| Audio Recording | sounddevice |
| Audio Processing | NumPy, wave |

## System Prompt

The assistant is configured as "Sandy", a receptionist at Vancouver Dental Clinic with knowledge of:
- Operating hours: Mon-Fri 8AM-6PM, Sat 9AM-3PM
- Services: General dentistry, cleaning, fillings, crowns, root canals, cosmetic dentistry
- Location and contact information

## Required Files

Vosk Arabic Model: Download from Vosk Models (vosk-model-ar-0.22)
Place the model folder in the project directory or Downloads folder

## How It Works

Speech Recognition: User speaks → Vosk converts Arabic speech to text
AI Processing: Text → OpenRouter LLM generates contextual response
Text-to-Speech: Response → gTTS converts to Arabic audio
Interface: Streamlit displays chat history and plays audio

## Author
Fatma Abdullah

```bash
pip install streamlit sounddevice numpy vosk gtts openai
