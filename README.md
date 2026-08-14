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

### 1. Install or Reference the Skill

* **Option A: Install globally (all projects)**
  ```bash
  git clone https://github.com/nroadley/Creating-Oneshot-Hero-Landing-Pages.git ~/.gemini/config/skills/creating-oneshot-landing-pages
  ```

* **Option B: Install to your current workspace only**
  Inside your project root:
  ```bash
  git clone https://github.com/nroadley/Creating-Oneshot-Hero-Landing-Pages.git .agents/skills/creating-oneshot-landing-pages
  ```

* **Option C: Run directly via chat URL (Zero install)**
  Ask your agent to read the repository directly in your prompt:
  > *"Read https://github.com/nroadley/Creating-Oneshot-Hero-Landing-Pages/blob/main/SKILL.md and build a landing page for Lumina acoustic guitars."*

---

### 2. Prompt Your Agent

Once installed, you can invoke the skill via its slash command or by asking naturally:

* **Using the Slash Command:**
  ```text
  /creating-oneshot-landing-pages <your prompt>
  ```
  *Example:*
  ```text
  /creating-oneshot-landing-pages Build a launch landing page for Lumina — an acoustic guitar workshop handcrafting instruments from reclaimed Pacific Northwest cedar.
  ```

* **Or Natural Prompts:**
  > *"Create a hero landing page for Nomad Foils, a company designing electric carbon-fiber hydrofoil boards for open-ocean riding."*

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
