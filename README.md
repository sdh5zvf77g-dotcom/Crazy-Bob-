# Crazy Bob 🤪

Private local AI chat that runs entirely in your browser using WebLLM + WebGPU.  
No cloud. No API keys. Works on iPhone (Safari 26+).

## Features

- **Single mode** – normal chat
- **Team mode** – three agents collaborate:
  - **Planner** – analyses & plans
  - **Writer** – drafts letters / advice
  - **Reviewer** – polishes the final result
- Fully offline after the first model download
- Installable as a Home Screen app on iPhone

## Live demo (after you enable GitHub Pages)

Once you push this repo and turn on Pages, open:

```
https://YOUR-USERNAME.github.io/crazy-bob/
```

## How to put it on GitHub

1. Create a new repository named `crazy-bob` (public is easiest for Pages).
2. Upload these three files to the root of the repo:
   - `index.html`
   - `apple-touch-icon.png`
   - `crazy-bob-icon.png`
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
