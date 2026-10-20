# Crazy Bob 🤪

Private local AI chat that runs entirely in your browser using WebLLM + WebGPU.  
No cloud required for chat. Optional free API keys unlock richer web search. Works on iPhone (Safari 26+).

## Features

### Core
- **Single mode** – normal chat
- **Team mode** – three agents collaborate:
  - **Planner** – analyses & plans
  - **Writer** – drafts letters / advice
  - **Reviewer** – polishes the final result
- **Persistent chat history** – saved on device (IndexedDB); last ~80 messages kept
- Fully offline after the first model download (except optional online tools)
- Installable as a Home Screen app on iPhone
- Clear history (trash icon)

### Voice
- **🎤 Talk** – speech-to-text input (tap mic)
- **Bob talks back** – text-to-speech with voice picker, speed control
- **Continuous conversation** – after Bob speaks, auto-listen again (Settings)
- Listening language selectable (English, Thai, Spanish, French, German, Japanese, Chinese…)

### Online tools (need internet)
| Chip | What it does | Needs key? |
|------|----------------|------------|
| 📰 Today's news | BBC + Reuters + NPR headlines | No |
| 🔍 Research a topic | Wikipedia + DuckDuckGo Instant Answer (+ web search if key) | Optional |
| 🌐 Search the web | Live web results via Tavily or Serper | Yes (free tiers) |
| 🌤️ Weather | Any city via Open-Meteo | No |
| 💱 Currency | Live FX rates (frankfurter.app / ECB) | No |
| 📈 Crypto | Price + 24h change (CoinGecko) | No |
| 📖 Define | Dictionary definitions | No |
| 🌍 Translate | Free translation (MyMemory) | No |
| 🔗 Summarize URL | Fetch page text & summarise | No |

**Optional API keys** (Settings → Online search):
- [Serper.dev](https://serper.dev) — 2,500 free Google searches
- [Tavily](https://tavily.com) — 1,000 free searches/month, great for AI

Keys are stored **only on this device**.

### Quality-of-life
- Markdown rendering in replies (lists, bold, code)
- Copy / Speak buttons on every assistant message
- **Stop** button while generating
- Personality presets (Classic, Calm, Coach, Formal, Witty)
- Export chat as text file
- Auto-restore last model on open

## Use on iPhone

1. Open the GitHub Pages URL in **Safari**.
2. Tap **Share → Add to Home Screen**.
3. It appears as **Crazy Bob** with the crazy face icon.
4. Choose a model (Llama 3.2 1B recommended) → **Load**.
5. Switch to **Team** mode if you want the three agents.
6. Tap **⚙️** for voice, personality, continuous chat, and optional API keys.
7. Tap **🎤** to talk; allow microphone when asked.
8. Use the chips for news, research, web search, weather, currency, crypto, define, translate, or URL summarise.

## Models

| Model              | Size     | Notes                        |
|--------------------|----------|------------------------------|
| SmolLM2 360M       | ~210 MB  | Fastest                      |
| Llama 3.2 1B       | ~700 MB  | Best balance (recommended)   |
| Qwen2.5 0.5B       | ~280 MB  | Very light                   |
| Llama 3.2 3B       | ~1.8 GB  | Higher quality, more memory  |

First load downloads the model (cached afterwards). Needs WebGPU (Safari 26+ or recent Chrome).

## Privacy

Chat runs on your device. Conversations never leave your phone unless you use an online tool (news, search, weather, etc.), in which case only that query/URL is sent to the respective free public API. Optional API keys stay in local storage.

---

Made for fun. Stay crazy.
