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
  - You need either an OpenAI API Key or Google Gemini API Key.
  - Optional: Google API Key + Custom Search Engine ID for web search.

  Install

  - Download the DMG from Release/Assets and drag ADA to Applications.
  - Open ADA and add your API keys in Settings.
  - First launch may take up to a minute while components warm up.

  Privacy

  - Your documents are processed locally. Calls to AI or search providers are made only when you use those features, with the keys you provide.

  Troubleshooting

  - At first launch, MacOS Gatekeeper might block the app.
    <img width="372" height="392" alt="Screenshot 2025-12-22 at 11 24 25 AM" src="https://github.com/user-attachments/assets/56a20ca8-c309-485c-937e-c0f36f23ea7c" />

    If this window pops up, click `Cancel`, then open Terminal, then copy and paste this:

    `xattr -dr com.apple.quarantine "/Applications/ADA.app"`

    Then try to launch it again.

  - Slow first start: allow up to 60 seconds on initial launch.
  - Voice chat not connecting: confirm your API keys in Settings and microphone permission is granted.
  - Still stuck? Quit ADA, reopen, and try again after confirming your keys.
  
