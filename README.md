# Chatbot with Avatar and Lipsync

An AI-powered **chatbot with a 3D avatar** capable of real-time lipsync, combining cutting-edge AI models with interactive 3D animation.

---

## 🎥 Demo
![Demo Screenshot](demo/screenshots/ui.png)

▶ **[Watch the full demo video](demo/demo.mp4)**

---

## ✨ Key Features
- **Real-time Lipsync:** Avatar powered by Unity + SALSA Suite.
- **AI Chatbot:** Text & voice input supported.
- **Voice Pipeline:**
  - **Speech-to-Text:** Whisper Large v3
  - **LLM Chatbot:** Mistral Nemo (OpenRouter)
  - **Text-to-Speech:** `tts_models/en/vctk/vits`
- **Backend:** FastAPI running on Kaggle (GPU for Whisper + TTS).
- **Frontend:** React page, connected via LocalTunnel.
- **Avatar Fetch System:** Custom C# script with timestamp mechanism to avoid repeated audio fetching.

---

## 🏗 Architecture
```mermaid
graph TD
A[Voice/Text Input] --> B[LangGraph Flow]
B --> C[Chatbot Response]
C --> D[TTS Audio Generation]
D --> E[FastAPI Server]
E --> F[Unity Avatar (fetches audio + lipsync)]
