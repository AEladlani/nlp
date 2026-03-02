# Notebook: TTS & STT with AI Voice Detection

This notebook provides a complete workflow for analyzing, generating, and transcribing speech. It combines **AI voice detection**, **text-to-speech (TTS)**, and **speech-to-text (STT)** capabilities in one interactive environment.

---

## Features

### 1. AI Voice Detection
The notebook can analyze an audio file and determine whether the voice is **AI-generated or human**. It evaluates characteristics such as pitch variation, spectral features, and the presence of silence gaps. The result includes a classification along with an explanation of why the audio was identified as human or AI-generated.

---

### 2. Text-to-Speech (TTS)
The notebook supports converting text into spoken audio in both **English and French**. Users can input any text, and the notebook generates a natural-sounding audio file that can be played or saved for later use.

---

### 3. Speech-to-Text (STT)
The notebook provides transcription of spoken language into text, both from **pre-recorded audio files** and **live microphone input**.  
- For live input, it continuously captures audio, detects when the user is speaking, and generates a real-time transcript.  
- Recording automatically stops after a period of silence, making the transcription process seamless and efficient.

---

## Workflow
1. Analyze an audio file to check if the voice is AI-generated or human.  
2. Convert text into speech in English or French.  
3. Transcribe speech from audio files or live microphone input into text.

---

## Notes
- The AI voice detection is heuristic and provides an estimation rather than a definitive classification.  
- Live transcription adapts to voice activity and pauses to provide accurate real-time results.  
- The notebook allows users to experiment with both generating speech and understanding audio in a single environment.
