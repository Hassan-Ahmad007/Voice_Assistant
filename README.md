# 🎙️ AI Voice Assistant

A seamless, real-time AI Voice Assistant that listens to your speech, processes it through a Large Language Model (LLM), and responds back with a synthesized voice. This project features a modern, glassmorphism-inspired UI and is designed to run efficiently in Google Colab or as a standalone Gradio app.

## 🚀 Live Demo

You can interact with the live application here:
**[https://huggingface.co/spaces/hassan121ahmad/AI_Voice_Assistant]**

## ✨ Features
- **Automatic Speech Recognition (ASR):** Powered by `faster-whisper` for high-speed, accurate transcription.
- **Intelligence:** Uses Groq's Llama-3.1-8b-instant model for near-instantaneous responses.
- **Text-to-Speech (TTS):** Converts AI responses back to audio using Google Text-to-Speech (gTTS).
- **Modern UI:** Built with Gradio featuring a custom CSS theme with gradients and glassmorphism effects.
- **Hands-Free Experience:** The app automatically triggers processing as soon as audio is captured.

## 🛠️ Tech Stack
- **UI Framework:** [Gradio](https://gradio.app/)
- **Speech-to-Text:** [faster-whisper](https://github.com/SYSTRAN/faster-whisper)
- **Inference Engine:** [Groq Cloud API](https://groq.com/)
- **LLM:** Meta Llama 3.1 8B
- **Text-to-Speech:** [gTTS](https://pypi.org/project/gTTS/)
- **Runtime:** Python / Google Colab

## ⚙️ Setup & Installation

To run this locally or in Colab, you will need a **Groq API Key**. 

1. **Install Dependencies:**
   ```bash
   pip install faster-whisper groq gtts gradio
   ```

2. **Set Environment Variables:**
   Ensure you have your `GROQ_API_KEY` available in your environment or Colab secrets.

3. **Run the Application:**
   Execute the Python script to launch the Gradio interface.

## 📝 How It Works
1. **Capture:** The user records audio through the microphone input.
2. **Transcribe:** `faster-whisper` converts the audio data into text.
3. **Think:** The text is sent to the Llama model via Groq API to generate a response.
4. **Speak:** `gTTS` generates an MP3 file of the response text.
5. **Output:** The UI displays the transcription, the AI's text, and automatically plays the audio response.
