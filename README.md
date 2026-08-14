# Creating Oneshot Hero Landing Pages 🚀

An **Antigravity (AGY)** skill to plan, design, and build video-driven parallax hero landing pages using video scrubbing.

---

## 📋 Prerequisites

1. **Antigravity (AGY)** *(Recommended)*: Works out of the box with Antigravity. Can also run in other agent environments with minor adaptations.
2. **Gemini API Key**: Required for Omni video generation. Get a key at [Google AI Studio](https://aistudio.google.com/apikey).
   ```bash
   export GEMINI_API_KEY="your-gemini-api-key"
   ```

---

## ⚡ Quickstart

### 1. Install or Provide the Skill

You can install the skill permanently or paste it into your chat:

* **Option A: Add to your Antigravity skills directory**
  ```bash
  mkdir -p ~/.gemini/skills/creating-oneshot-landing-pages
  cp SKILL.md ~/.gemini/skills/creating-oneshot-landing-pages/
  ```
  *(Or place `SKILL.md` in your workspace at `.agents/skills/creating-oneshot-landing-pages/`)*

* **Option B: Copy & paste directly**
  Copy the contents of [`SKILL.md`](SKILL.md) and paste it directly into your prompt along with your request.

---

### 2. Prompt Your Agent

Give your agent a clear product or brand idea:

> *"Build a launch landing page for Lumina — an acoustic guitar workshop handcrafting instruments from reclaimed Pacific Northwest cedar and redwood."*

> *"Create a hero page for Nomad Foils, a company that designs electric carbon-fiber hydrofoil boards for open-ocean riding."*

> *"Make a landing page for our small-batch ceramic studio based in Kyoto, showcasing wood-fired matcha bowls and handcrafted teaware."*

---

## 🛠️ How It Works

1. **Reference Images**: Generates reference images using Nano Banana (`gemini-3.1-flash-image`).
2. **Video Generation**: Calls `gemini-omni-flash-preview` to generate 10s 16:9 `.mp4` video assets in `./assets/`.
3. **Frontend Implementation**: Builds a 400vh sticky video-scrubbing layout (`index.html`) with progress-locked typography and clean design rules (no unnecessary icons, fake tickers, or toy widgets).
4. **Local Preview**: Launches a local preview server so you can test the live page immediately.

---

## 📄 License

[MIT](LICENSE)
