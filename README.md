# ADA-Electron
 Overview
  Local real‑time voice assistant with camera, chat widget, and a document reader (EPUB/PDF/TXT/DOCX). Uses local STT/TTS (Moonshine + Kokoro) and OpenAI for LLM. Embeddings/ChromaDB have been removed; the library uses a fast keyword search by default.

  Highlights

  - Conversational Assistant: Voice or text chat with a responsive avatar.
  - Ask Your Documents: Import EPUB/PDF/DOCX/TXT and ask questions about them.
  - Read Aloud: Natural text‑to‑speech with on‑screen captions.
  - Smart Resume: Remembers where you left off in a document.
  - Clean UI: Distraction‑free chat and document views.

  Requirements

  - macOS (Apple Silicon).
  - One provider key for chat (OpenAI or Google Gemini).
  - Optional: Google API Key + Custom Search Engine ID for web search.

  Install

  - Download the DMG from Assets and drag ADA to Applications.
  - Open ADA and add your API keys in Settings.
  - First launch may take up to a minute while components warm up.

  Privacy

  - Your documents are processed locally. Calls to AI or search providers are made only when you use those features, with the keys you provide.

  Troubleshooting

  - Slow first start: allow up to 60 seconds on initial launch.
  - Voice chat not connecting: confirm your API keys in Settings and microphone permission is granted.
  - Still stuck? Quit ADA, reopen, and try again after confirming your keys.
