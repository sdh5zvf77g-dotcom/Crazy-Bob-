# Crazy Bob 🤪

Private local AI chat that runs entirely in your browser using WebLLM + WebGPU.  
No cloud required for chat. Optional free API keys unlock richer web search. Works on iPhone (Safari 26+).

## Features

- **Single mode** – normal chat
- **Team mode** – three agents collaborate:
  - **Planner** – analyses & plans
  - **Writer** – drafts letters / advice
  - **Reviewer** – polishes the final result
- **Voice conversation** – tap the mic 🎤 to talk; Crazy Bob can speak replies out loud
- **Voice settings** – choose system voice, speaking speed, and listening language (⚙️ button)
- **Online tools** (need internet):
  - 📰 Multi-source news (BBC, Reuters, NPR)
  - 🔍 Research a topic (Wikipedia + DuckDuckGo Instant Answer)
  - 🌐 Web search (optional free API keys: Serper or Tavily)
  - 🌤️ Weather (Open-Meteo, any city)
- **Optional API keys** in Settings for richer web search (keys stored only on this device)
- **Persistent chat history** – conversations are saved on the phone (IndexedDB) so Bob remembers past chats
- Fully offline after the first model download (voice uses the device’s built-in speech engines)
- Installable as a Home Screen app on iPhone
- Clear history button (trash icon) if you want to wipe saved chats

## Live demo (after you enable GitHub Pages)

Once you push this repo and turn on Pages, open:

```
https://YOUR-USERNAME.github.io/crazy-bob/
```

## How to put it on GitHub

1. Create a new repository named `crazy-bob` (public is easiest for Pages).
2. Upload these files to the root of the repo:
   - `index.html`
   - `apple-touch-icon.png`
   - `crazy-bob-icon.png`
   - `manifest.json`
   - `README.md`
3. Go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`.
6. Save. After 1–2 minutes your site will be live at:
   `https://YOUR-USERNAME.github.io/crazy-bob/`

## Use on iPhone

1. Open the GitHub Pages URL in **Safari**.
2. Tap **Share → Add to Home Screen**.
3. It appears as **Crazy Bob** with the crazy face icon.
4. Choose a model (Llama 3.2 1B recommended) → **Load**.
5. Switch to **Team** mode if you want the three agents.
6. Tap **⚙️** to pick a voice, turn “Crazy Bob talks back” on/off, and optionally paste free Serper or Tavily API keys for web search.
7. Tap the **🎤** mic button, speak, then Bob will reply (and speak if enabled). Allow microphone access when Safari asks.
8. Use the chips for news, research, web search, or weather.

## Memory notes

- Chat history is stored locally in the browser (IndexedDB) on your phone.
- Last ~80 messages are kept so storage stays reasonable.
- The model itself is also cached after the first download.
- Use the trash icon to clear all saved chats if needed.
- History is tied to the site origin (your GitHub Pages URL).

## Models

| Model              | Size     | Notes                        |
|--------------------|----------|------------------------------|
| SmolLM2 360M       | ~210 MB  | Fastest                      |
| Llama 3.2 1B       | ~700 MB  | Best balance (recommended)   |
| Qwen2.5 0.5B       | ~280 MB  | Very light                   |
| Llama 3.2 3B       | ~1.8 GB  | Higher quality, more memory  |

First load downloads the model (cached afterwards). Needs WebGPU (Safari 26+ or recent Chrome).

## Privacy

Everything runs on your device. Conversations never leave your phone.

---

Made for fun. Stay crazy.
