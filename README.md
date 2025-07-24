# Chatbot with Avatar and Lipsync

An AI-powered **chatbot with a 3D avatar** capable of real-time lipsync, combining cutting-edge AI models with interactive 3D animation.

---

## 🎥 Demo
![Demo Screenshot](Demo/Visuals/UI.png)

▶ **[Watch the full demo video](https://drive.google.com/drive/folders/1cbmHQgFHpF2Sk_7kZcn62mFdfi4xsxI3?usp=sharing)**

---

## ✨ Key Features
- **Real-time Lipsync:** Avatar powered by Unity + SALSA Suite.
- **AI Chatbot:** Text & voice input supported.
- **Voice Pipeline:**
  - **Speech-to-Text:** Whisper Large v3
  - **LLM Chatbot:** Mistral Nemo (OpenRouter)
  - **Text-to-Speech:** `tts_models/en/vctk/vits`
- **Backend:** FastAPI running on Kaggle and exposed via **LocalTunnel**.
- **Frontend:** React page.
- **Audio Fetch System:** A **custom Unity C# script** automatically fetches the latest audio response from **backend**.

---


## 🧠 LangGraph Flow
This project uses **LangGraph** to manage the chatbot's conversational flow.

➡ [**View the Full LangGraph Flow Here**](Langgraph/langgraph_flow.png)

---

## 🛠 Tech Stack
- **Unity + SALSA Suite** – Avatar and real-time lipsync.
- **LangGraph** – Conversation flow.
- **FastAPI** – Backend server for chatbot logic and audio processing.
- **React** – Frontend UI for user input.
- **Kaggle GPU** – For Whisper & TTS.
- **LocalTunnel** – Free server exposure.
- **Models:**
  - Whisper Large v3
  - Mistral Nemo (OpenRouter)
  - VITS TTS (tts_models/en/vctk/vits)



---

## 📌 How It Works
1. User speaks or types a message.
2. LangGraph processes the input and generates a chatbot response.
3. Response is converted to speech (TTS).
4. Unity Avatar fetches the audio file and performs lipsync using SALSA Suite.

---

## 🙏 Acknowledgements & Inspiration
This project was inspired by the incredible work of [Wassim SAMAD](https://github.com/wass08).  
His projects and ideas on 3d avatars motivated me to build my own chatbot with a 3D avatar and lipsync.

---

## 💡 Final Note
This project was built entirely using **open-source models** and **free servers** (Kaggle for GPU, LocalTunnel for exposure).  
I hope this demonstrates that you can build high-quality, innovative projects **without spending a lot of money**—just with creativity, persistence, and open tools.

---

## 📄 License
This repository is a **showcase project**.  
The source code is **proprietary and not publicly available**, but you are welcome to explore the architecture, demo, and ideas.

