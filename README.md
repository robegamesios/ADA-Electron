# ADA-Electron
  Overview
  Local real‑time voice assistant with camera, chat widget, and a document reader (EPUB/PDF/TXT/DOCX). Uses local STT/TTS (Moonshine + Kokoro) and OpenAI or Gemini for LLM. 
  
  Highlights

  - Conversational Assistant: Voice or text chat with a responsive avatar.
  - Perform web search: e.g. ask about the weather, directions, latest news.
  - Conversation history: Restore old conversations and continue where you left of.
  - Vision queries: Turn on the camera and ask what the avatar sees.
  - Book Reader: Import EPUB/PDF/DOCX/TXT, listen with natural captions, search quickly, and resume exactly where you left off.
  - Ask about your documents: e.g. summarize a chapter in the book.

  Powered By

  - Avatar: TalkingHead by met4citizen — https://github.com/met4citizen/TalkingHead
  - Real‑time pipeline: Pipecat — https://github.com/pipecat-ai/pipecat
  - Text‑to‑Speech: KokoroTTS (ONNX)
  - Speech‑to‑Text: Moonshine (ONNX)

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
  - If Gatekeeper is flagging the app and it says it's damaged when you run the app, do this in terminal:

    xattr -dr com.apple.quarantine "/Applications/ADA.app"
