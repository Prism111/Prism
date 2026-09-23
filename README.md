# Prism

**Turn a conversation into a movie.**

Talk to an AI. Build your story. Generate the scenes. Create the film.

Prism is a free, open-source desktop AI filmmaking studio that turns your ideas into long-form, character-consistent videos and movies — from a 30-second commercial to a full multi-act film.

[**⬇ Download Prism**](https://github.com/Prism111/Prism/releases/download/v1.0.0/Prism.Setup.1.0.0.exe)

---

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/f7aa8b71-adf4-424b-b7b9-e574bc14a56a" />



---

## Why Prism

Most AI video tools generate isolated 3–5 second clips that drift: characters change faces, outfits swap mid-scene, backgrounds shift, camera motion feels random. There's no story, just clips.

Prism is built to act as an **AI Director and full production studio**, not a clip generator:

- **Locks visual continuity** — characters, wardrobe, props, and locations stay consistent scene to scene.
- **Scales to any runtime** — from a 30-second short to a 90-minute film, built from rolling 15-second production blocks.
- **Automates the full pipeline** — story development, casting, visual asset creation, scene-by-scene cinematography, lip-synced dialogue, and final post-production stitching.
- **Runs entirely on your machine** — your generated media never leaves your device.
- **Bring your own API keys** — works with Gemini, GPT, Claude, and Grok.

## How it works

1. **Talk to the AI Director** — describe your movie: genre, characters, tone, runtime. Attach scripts, concept art, or voice notes if you want.
2. **Generate the blueprint** — type `generate plan` and Prism drafts a full Master Production Blueprint: cast, sets, key props, and a scene-by-scene timeline with camera direction.
3. **Review the visual board** — inspect AI-generated character turnarounds, wardrobe sheets, and environment plates. Regenerate or tweak anything in plain language (e.g. *"give Dr. Marcus grey hair"*).
4. **Produce** — type `continue` and Prism renders each 15-second scene, using the previous scene's video as a reference for the next so lighting, motion, and continuity carry through automatically.
5. **Get your movie** — Prism stitches every scene into a single `master_movie.mp4` with normalized video/audio, ready to watch or export.

You can pause and resume production at any time without losing progress, and regenerate a single scene without re-rendering the rest of the movie.

## Features

| Feature | Description |
|---|---|
| Unlimited project length | Films are built from modular 15-second scenes organized into acts |
| Visual asset conditioning | 2K character turnarounds, wardrobe sheets, prop and set plates |
| Video reference chaining | Each new scene references the prior scene's video to guarantee continuity |
| Native voice & lip-sync | Dialogue and lip motion generated automatically, no separate dubbing step |
| Surgical scene regeneration | Edit and re-render a single scene via natural language |
| Pre-flight checks | Estimates disk space and API credit cost before rendering starts |
| Multi-LLM support | Google Gemini, OpenAI GPT, Anthropic Claude, and xAI Grok |
| Multimodal input | Text, voice notes, reference images, and story documents |

## Installation

1. Download the installer from the [latest release](https://github.com/Prism111/Prism/releases/tag/v1.0.0) (`Prism.Setup.1.0.0.exe`, ~126 MB).
2. Run the installer. Windows SmartScreen may show **"Windows protected your PC"** — click **More info → Run anyway** to proceed. This appears because the installer isn't yet code-signed, not because of any threat.
3. Launch Prism and add your API key(s) for whichever provider(s) you want to use (Gemini, OpenAI, Anthropic, or xAI). Keys are encrypted locally via OS-level secure storage and never leave your device.

## Requirements

- Windows (installer provided). Generated media, projects, and history are stored locally under `Documents/Prism/`.
- Your own API key for at least one supported provider (Gemini, GPT, Claude, or Grok).
- FFmpeg is bundled — no separate install needed.

## Tech stack

Electron · Next.js / React · FFmpeg · Zod-validated LLM pipeline

## Roadmap / feedback

Prism is early (v1.0.0) and actively developed. Bug reports, feature requests, and ideas are welcome — open an [issue](../../issues) or start a [discussion](../../discussions).

## Contact

Prism3157@gmail.com

## License

MIT — see [LICENSE](LICENSE).
