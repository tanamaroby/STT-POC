---
title: STT POC
emoji: 👁
colorFrom: indigo
colorTo: gray
sdk: gradio
sdk_version: 5.34.2
app_file: app.py
pinned: false
short_description: Proof of concept for speech to text and transcriber
---

Check out the configuration reference at https://huggingface.co/docs/hub/spaces-config-reference

# Whisper Speech-to-Text Web App

Welcome! This repository provides a simple, self-hosted web application for automatic speech recognition (ASR) using OpenAI's Whisper model (large-v3), powered by Gradio.  
Developed and maintained by **Roby Tanama, CTO of Trietech Private Limited**.

## Features

- **Multilingual Speech-to-Text:** Transcribe audio in many languages using Whisper's advanced multilingual capabilities.
- **Upload-Only Interface:** For stability, the app only accepts audio file uploads (no in-browser recording).
- **Runs Locally:** All processing happens on your machine—no cloud required.
- **Easy to Use:** Minimal setup with Python and pip.

## Quickstart: Self-Hosting Tutorial

Follow these steps to run the app on your own computer.

### 1. Clone the Repository

```bash
git clone https://github.com/tanamaroby/STT-POC.git
cd STT-POC
```

### 2. Create and Activate a Virtual Environment

**On macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

**On Windows:**
```cmd
python -m venv venv
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Run the Application

```bash
python app.py
```

- The Gradio web interface will launch and display a local URL (e.g., http://127.0.0.1:7860/).
- Open this URL in your browser.

## Usage

1. **Upload an audio file** (WAV, MP3, etc.) using the upload button.
2. Wait for the transcription to complete.
3. Copy or use the recognized text as needed.

## Notes

- **First run may take time** as the model is downloaded (~2GB).
- **Supports many languages** thanks to Whisper's multilingual model.
- **No recording feature**: For stability, only file upload is enabled.
- **GPU recommended** for faster transcription, but CPU is supported.

## About

Developed by **Roby Tanama, CTO of Trietech Private Limited**.

Get started and enjoy high-quality speech-to-text in your browser, on your own machine!
