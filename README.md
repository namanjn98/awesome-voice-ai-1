<div align="center">

# Awesome Voice AI

[![Awesome](https://img.shields.io/badge/Awesome-Voice_AI-E8C98A?style=for-the-badge&labelColor=0B0B0C&logo=awesomelists)](https://github.com/Mirror-Corporation/awesome-voice-ai)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-6EA8FF?style=for-the-badge&labelColor=0B0B0C)](#contributing)
[![maintained by](https://img.shields.io/badge/maintained_by-Mirror_Corporation-F4F4EF?style=for-the-badge&labelColor=0B0B0C)](https://github.com/Mirror-Corporation)

**A curated list of voice AI: tools, models, datasets, papers, products, and ideas.**
*Maintained by [Mirror Corporation](https://github.com/Mirror-Corporation) — we live in this space.*

</div>

<br/>

> **Scope.** Voice cloning, TTS, ASR, voice agents, voice memory, voice-first UX.
> **Bias.** Things we have used, products we have shipped against, papers we have read.
> **Not on this list.** Generic LLM tooling, image generation, anything without a voice angle.

<br/>

## Contents

- [Text-to-speech & voice cloning](#text-to-speech--voice-cloning)
- [Speech recognition (ASR)](#speech-recognition-asr)
- [Voice agents & runtimes](#voice-agents--runtimes)
- [Open-source models](#open-source-models)
- [Datasets](#datasets)
- [Voice-first products](#voice-first-products)
- [Memory & retrieval for voice](#memory--retrieval-for-voice)
- [Research & papers](#research--papers)
- [Ethics & safety](#ethics--safety)
- [Communities](#communities)
- [Contributing](#contributing)

<br/>

## Text-to-speech & voice cloning

| Tool | What it is | Why it matters |
|---|---|---|
| [ElevenLabs](https://elevenlabs.io/) | hosted TTS + voice cloning | current quality leader for emotional control |
| [PlayHT](https://play.ht/) | hosted TTS | strong multilingual, low latency |
| [Cartesia · Sonic](https://cartesia.ai/sonic) | low-latency TTS | sub-100ms first audio, best-in-class for live agents |
| [Coqui TTS](https://github.com/coqui-ai/TTS) | open-source TTS toolkit | the go-to self-host TTS for many years |
| [XTTS-v2](https://huggingface.co/coqui/XTTS-v2) | open multilingual voice clone | zero-shot voice cloning from a 6-second sample |
| [F5-TTS](https://github.com/SWivid/F5-TTS) | open flow-matching TTS | fast, expressive, easy fine-tuning |
| [OpenVoice](https://github.com/myshell-ai/OpenVoice) | open voice cloning | tone + accent + emotion controls |

## Speech recognition (ASR)

| Tool | What it is |
|---|---|
| [Whisper](https://github.com/openai/whisper) | OpenAI's open ASR — the baseline everyone benchmarks against |
| [Whisper.cpp](https://github.com/ggerganov/whisper.cpp) | C/C++ port of Whisper — runs on consumer hardware |
| [Faster Whisper](https://github.com/SYSTRAN/faster-whisper) | optimized Whisper with CTranslate2 — 4× speedup |
| [Deepgram](https://deepgram.com/) | hosted ASR — best latency on streaming |
| [AssemblyAI](https://www.assemblyai.com/) | hosted ASR + speaker diarization + sentiment |
| [Distil-Whisper](https://github.com/huggingface/distil-whisper) | smaller, faster Whisper — 6× smaller, 5× faster |

## Voice agents & runtimes

| Tool | What it is |
|---|---|
| [LiveKit Agents](https://docs.livekit.io/agents/) | open framework for real-time voice agents over WebRTC |
| [Vapi](https://vapi.ai/) | hosted voice agent platform — fast prototyping |
| [Pipecat](https://github.com/pipecat-ai/pipecat) | open-source pipeline framework for voice AI |
| [Retell AI](https://www.retellai.com/) | hosted voice agent — telephony-first |
| [Bland AI](https://bland.ai/) | hosted voice agent — focused on phone calls |
| [Daily.co Bots](https://www.daily.co/products/voice-and-video-bots/) | conversation infrastructure for voice bots |
| [Tazo Labs](https://tazolabs.com/) | speech-to-decision models for voice agents, cut voice LLM costs by 50% |

## Open-source models

- [Llama 3 family](https://llama.meta.com/) — Meta, the strongest open chat backbone
- [Qwen 2 / Qwen 2.5](https://github.com/QwenLM/Qwen2) — Alibaba, strong multilingual reasoning
- [DeepSeek-V3](https://github.com/deepseek-ai/DeepSeek-V3) — best open reasoning model of 2025
- [Mistral Small / Large](https://mistral.ai/) — solid open-weight European alternative

## Datasets

- [LibriTTS](https://www.openslr.org/60/) — 585h English audiobook speech, multi-speaker
- [Common Voice](https://commonvoice.mozilla.org/) — Mozilla's multilingual crowdsourced speech corpus
- [VoxCeleb 1/2](https://www.robots.ox.ac.uk/~vgg/data/voxceleb/) — celebrity voices for speaker recognition
- [VCTK](https://datashare.ed.ac.uk/handle/10283/3443) — 110 English speakers, studio quality
- [LJSpeech](https://keithito.com/LJ-Speech-Dataset/) — 13k clips, single speaker — the TTS hello-world

## Voice-first products

| Product | Category | Note |
|---|---|---|
| [Mirror](https://mirror-ai.app) | digital immortality, heritage voice | shipping today; we make it |
| [Suno](https://suno.com/) | voice-to-song generation | the standard for AI music |
| [Udio](https://www.udio.com/) | AI music generation | strongest competitor to Suno |
| [Pi (Inflection)](https://pi.ai/) | voice companion | one of the first voice-native AI products |
| [Friend / Limitless](https://www.limitless.ai/) | wearable voice memory | continuous capture + recall |

## Memory & retrieval for voice

- [Mem0](https://github.com/mem0ai/mem0) — open long-term memory layer for AI agents
- [Zep](https://github.com/getzep/zep) — long-term memory + retrieval for chat & voice
- [LangMem](https://github.com/langchain-ai/langmem) — memory primitives for LangGraph
- [Chroma](https://www.trychroma.com/) — open vector DB, common backend
- [LanceDB](https://lancedb.com/) — embedded vector DB, fast for local

## Research & papers

- 📄 **NaturalSpeech 3 (2024)** — factorized diffusion for prosody
- 📄 **StyleTTS 2 (2023)** — diffusion for expressive TTS
- 📄 **Voicebox (Meta, 2023)** — text-guided multilingual generation
- 📄 **AudioLM (Google, 2022)** — language modeling for audio
- 📄 **NaturalSpeech 2 (Microsoft, 2023)** — latent diffusion TTS
- 📄 **SoundStream (Google, 2021)** — the codec underneath modern audio LMs

## Ethics & safety

- [Partnership on AI — Synthetic Media](https://partnershiponai.org/workstream/synthetic-media/)
- [Coalition for Content Provenance and Authenticity (C2PA)](https://c2pa.org/)
- [DeepMedia Audio Detection](https://www.deepmedia.ai/)
- *On consent and the right to your own voice — see [Mirror Manifesto §VI](https://github.com/Mirror-Corporation/manifesto#vi--what-we-will-not-do).*

## Communities

- [Hugging Face — Audio](https://huggingface.co/audio)
- [LAION Discord — Audio](https://discord.gg/laion)
- [r/LocalLLaMA](https://www.reddit.com/r/LocalLLaMA/)

<br/>

## Contributing

Pull requests welcome. **Rules:**

1. Each entry needs **a one-line "why it matters."** No marketing copy.
2. We don't accept paid placements.
3. If you submit a product you built — say so in the PR.
4. If we remove your entry, we'll say why in the commit.

Open an issue if you disagree with a removal — we read everything.

<br/>

---

<div align="center">

<sub><b>Awesome Voice AI</b> · maintained by <a href="https://github.com/Mirror-Corporation">Mirror Corporation</a></sub>
<br/>
<sub><a href="https://mirror-ai.app">mirror-ai.app</a> · <a href="mailto:aimirror630@gmail.com">aimirror630@gmail.com</a></sub>

</div>
