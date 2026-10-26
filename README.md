# Prism

**Turn a conversation into a movie.**

Talk to an AI. Build your story. Generate the scenes. Create the film.

Prism is a free, open-source desktop AI filmmaking studio that turns your ideas into long-form, character-consistent videos and movies — from a 30-second commercial to a film of up to 30 minutes.

[**⬇ Download Prism**](https://github.com/Prism111/Prism/releases/download/v1.0.0/Prism-Setup-1.1.12.exe)

---

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/f7aa8b71-adf4-424b-b7b9-e574bc14a56a" />



---

## Why Prism

Most AI video tools generate isolated 3–5 second clips that drift: characters change faces, outfits swap mid-scene, backgrounds shift, camera motion feels random. There's no story, just clips.

Prism is built to act as an **AI Director and full production studio**, not a clip generator:

- **Locks visual continuity** — characters, wardrobe, props, and locations stay consistent scene to scene.
- **Scales from 30 seconds to 30 minutes** — built from rolling 15-second production blocks, planned one chapter at a time.
- **Automates the full pipeline** — story development, casting, visual asset creation, scene-by-scene cinematography, lip-synced dialogue, and final post-production stitching.
- **Keeps your projects on your computer** — projects, reference images, clips, and the finished movie are stored locally under `Documents/Prism/`.
- **Bring your own API keys** — a Javar AI key for images and video, plus a key for the AI Director (Gemini, GPT, Claude, or Grok).

## How it works

1. **Talk to the AI Director** — describe your movie: genre, characters, tone, runtime. You can attach scripts and story documents.
2. **Generate the blueprint** — type `generate plan` and Prism drafts a Master Production Blueprint: cast, sets, key props, and a scene-by-scene timeline with camera direction.
3. **Review the visual board** — inspect AI-generated character turnarounds, wardrobe sheets, and environment plates. Regenerate or tweak anything in plain language (e.g. *"give Dr. Marcus grey hair"*). Production only starts once every visual is approved.
4. **Produce** — click **Start Video Production** or type `continue`, and Prism renders each 15-second scene. Scenes that continue the same shot use the previous scene's video as a reference, so lighting, motion, and continuity carry through automatically.
5. **Get your movie** — Prism stitches every scene into a single `master_movie.mp4`, ready to watch or export.

You can pause and resume production at any time without losing progress, and regenerate a single scene without re-rendering the rest of the movie.

## Features

| Feature | Description |
|---|---|
| Up to 30 minutes | Films are built from modular 15-second scenes organized into chapters (10 minutes is the recommended length; 10–30 minutes is experimental) |
| Visual asset conditioning | 2K character turnarounds, wardrobe sheets, prop and set plates, all approved by you before rendering |
| Video reference chaining | Continuing scenes reference the prior scene's video; new locations start with a clean cut |
| Scene-to-scene hand-off | Every scene prompt states how the clip ends and how the next one begins |
| Distinct sound and scenes | The Director is instructed not to repeat actions, lines, sound effects, or music across scenes |
| Native voice & lip-sync | Dialogue and lip motion generated automatically, no separate dubbing step |
| Dailies (QC) | Review every generated clip with its exact prompt and reference images, and flag a clip to be re-rendered |
| Surgical scene regeneration | Edit and re-render a single scene via natural language |
| Pre-flight checks | Checks available disk space before rendering starts |
| Local logs | A built-in log folder button in Settings helps you diagnose problems; logs stay on your computer and your API keys are redacted |
| Multi-LLM support | Google Gemini, OpenAI GPT, Anthropic Claude, and xAI Grok |
| Light and dark themes | Switch from the sidebar |

## Installation

1. Download the installer from the [latest release](https://github.com/Prism111/Prism/releases/tag/v1.0.0) (`Prism-Setup-1.1.12.exe`, ~147 MB).
2. Run the installer. Windows SmartScreen may show **"Windows protected your PC"** — click **More info → Run anyway** to proceed. This appears because the installer isn't yet code-signed, not because of any threat.
3. Launch Prism, open **Settings**, and add your keys:
   - your **Javar AI** key (get one at [javarai.com](https://javarai.com)) — used to generate images and video;
   - a key for at least one AI Director provider (Gemini, OpenAI, Anthropic, or xAI).

   Keys are encrypted locally via OS-level secure storage and are stored only on your device.

## Requirements

- Windows (installer provided). Generated media, projects, and history are stored locally under `Documents/Prism/`.
- A [Javar AI](https://javarai.com) account and API key. Image and video generation use your own Javar AI credits; Javar AI sets its own pricing, so check its cost calculator before planning a long film.
- Your own API key for at least one supported AI Director provider (Gemini, GPT, Claude, or Grok).
- FFmpeg is bundled — no separate install needed.

## Tech stack

Electron · Next.js / React · FFmpeg · Zod-validated LLM pipeline

## Roadmap / feedback

Prism is early and actively developed. Bug reports, feature requests, and ideas are welcome — open an [issue](../../issues) or start a [discussion](../../discussions).

## Contact

Prism3157@gmail.com

## License

MIT — see [LICENSE](LICENSE).
