# ADA (Advanced Digital Assistant)

  An on‑device, voice‑first AI assistant with a 3D avatar. ADA reads your documents, answers questions, fetches weather and directions, searches the web, and holds natural conversations — all in a clean,
  focused UI.

  Youtube Video: https://youtu.be/IXWrxlnylsA?si=cD2n5kcS9doidNfX

  ### Highlights

  - Conversational Assistant: Voice or text chat with a responsive avatar and live captions.
  - Book Reader: Import EPUB/PDF/DOCX/TXT, listen with natural TTS, search quickly, and resume exactly where you left off.
  - Weather & Directions: Quick, natural queries for current conditions and routing via Google Maps.
  - Web Search: Fresh information and news when you need it.
  - Vision: Turn on your camera and ask ADA what it sees.
  - Hands‑Free Control: Say “Hey ADA” to wake; auto‑mutes after inactivity.

  ### Features

  - Voice Interaction
      - 2 Avatars to choose (ADA or ALAN) in Settings. Defaults to ADA.
      - Natural speech recognition (mic), realistic lip‑sync TTS, “Hey ADA” or "hey ALAN" wake word
      - Auto‑mute after 60s of silence; type in chat anytime
  - Document Intelligence
      - Formats: EPUB, PDF, DOCX, TXT
      - Read‑aloud, quick chapter/library keyword search, and Q&A over your uploads
  - Weather & Location
      - Current conditions, forecasts, location‑aware responses, natural questions
  - Navigation
      - Google Maps integration, route planning, distance/duration/traffic, voice prompts
  - Web Search
      - Real‑time results and news with basic source prioritization
  - Date & Time
      - World clock, date facts, friendly time calculations
  - Smart Agent
      - Context carry‑over within a session, multi‑domain switching, fallback to general knowledge

  ### Powered By

  - Avatar: TalkingHead by met4citizen — https://github.com/met4citizen/TalkingHead
  - Real‑time pipeline: Pipecat — https://github.com/pipecat-ai/pipecat
  - Text‑to‑Speech: KokoroTTS (ONNX)
  - Speech‑to‑Text: Moonshine (ONNX)

  ### Requirements

  - macOS (Apple Silicon).
  - One provider key for chat: OpenAI or Google Gemini.
  - Optional: Google API Key + Custom Search Engine ID (for web search).

  ### Install

  - Download the DMG from Releases and drag ADA to Applications.
  - Open ADA and add your API keys in Settings.
  - First launch may take up to a minute while components warm up.

  ### Privacy

  - Your documents are processed locally. Network calls only happen when you use LLM or web‑search features, with the keys you provide.

  ### Troubleshooting

  - Gatekeeper “App is damaged” (unsigned build)
    <img width="372" height="392" alt="Screenshot 2025-12-22 at 11 24 25 AM" src="https://github.com/user-attachments/assets/ded95df2-6e04-48e7-b24b-0f6b44f7762e" />

      - Quit ADA. In Terminal:
          - xattr -dr com.apple.quarantine "/Applications/ADA.app"
      - Launch again.
  - Slow first start
      - Allow up to 60 seconds on initial run (model warmup). Subsequent starts are faster.
  - Voice chat not connecting
      - Verify API keys in Settings; ensure microphone permission is granted.
  - Still stuck
      - Quit ADA, reopen, and try again after confirming keys.
