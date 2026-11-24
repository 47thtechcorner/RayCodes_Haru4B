# Haru-4B: Full-Duplex Speech-to-Speech Foundation Model

[![Haru 4B: World's First Real Time Voice AI at 65ms! (Local Setup)](https://img.youtube.com/vi/njrMzgHIXro/maxresdefault.jpg)](https://youtu.be/njrMzgHIXro)

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Model Size](https://img.shields.io/badge/Model%20Size-4B%20%2810.5%20GB%20BF16%29-indigo.svg)](https://huggingface.co/higurashi-ai/Haru-4B)
[![Frequency](https://img.shields.io/badge/Frame%20Rate-7.5%20Hz%20%28133%20ms%29-emerald.svg)](https://huggingface.co/higurashi-ai/Haru-4B)
[![Latency](https://img.shields.io/badge/Step%20Latency-15ms--65ms-cyan.svg)](https://huggingface.co/higurashi-ai/Haru-4B)
[![Footprint](https://img.shields.io/badge/Footprint-12GB%20VRAM%20%2F%20Apple%20MLX-orange.svg)](https://github.com/higurashi-ai/Haru)

> "Haru-4B by Higurashi AI is an open-weight, full-duplex speech-to-speech foundation model built on a Qwen3.5-4B backbone that listens and speaks simultaneously at 7.5 Hz (133 ms frames) across 9 languages, eliminating the awkward turn delays of traditional voice pipelines."

> 📺 **Watch the Full Video Walkthrough**: [Haru 4B: World's First Real Time Voice AI at 65ms! (Local Setup)](https://youtu.be/njrMzgHIXro)  
> ☕ **Support the Channel**: [https://ko-fi.com/prayasjain](https://ko-fi.com/prayasjain)

---

## 📊 Production Test Workflows

| Workflow | Capability Tested | Input Artifact | Expected Deliverable |
|---|---|---|---|
| **Real-Time Multilingual Backchanneling** | Generates spontaneous Hindi conversational fillers while continuously listening to English dialogue | Conversational English interview audio stream with natural pauses | Synthesized Hindi backchannel voice audio with natural filler words |
| **Live Call-Center Barge-In Stress Test** | Measures sub-150ms conversational interruption cutoff without end-of-turn detection delays | Urgent customer service interruption speech arriving mid-sentence | Truncated conversational agent voice audio demonstrating instant cutoff |
| **Dynamic Zero-Shot Voice Persona Swapping** | Preserves unique vocal timbre and pitch fidelity across emotional character prompts in 1 sampling step | Studio voice reference clips paired with expressive character cards | High-fidelity cloned persona voice audio with matched vocal timbre |

---

## ⚡ Quick Start (Windows PowerShell)

### Step 1: Setup Environment & Download Model Weights
```powershell
# Create and activate virtual environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1

# Install Haru and dependencies
pip install git+https://github.com/higurashi-ai/Haru.git
pip install torch torchaudio soundfile numpy

# Download Haru-4B model weights (10.5 GB BF16)
hf download higurashi-ai/Haru-4B --local-dir models/Haru-4B
```

### Step 2: Run Production Pipeline
```powershell
python main.py
```

---

## 🛠️ Practical Use Cases

- 🎙️ **Full-Duplex Customer Service Agents**: Eliminates awkward walkie-talkie pauses by instantly ceasing speech the exact millisecond a customer begins speaking.
- 🌐 **Simultaneous Cross-Lingual Interpretation**: Listens to live speech in one language while outputting translated conversational dialogue with natural acoustic fillers.
- 🎧 **Interactive Live Podcast Co-Hosts**: Acts as an engaged conversational partner that interjects spontaneous backchannel nods (*"uh-huh"*, *"right"*) without interrupting the primary speaker.
- 🕹️ **Zero-Latency Video Game Companions**: Delivers responsive non-player character dialogue with zero-shot voice cloning adapted dynamically from player audio clips.

---

## 🗺️ Future Feature Roadmap

- 🚀 **vLLM-Omni Serving Integration**: High-throughput multi-stream server configuration achieving 15 ms step latency across concurrent client calls.
- 🧠 **Instruction-Tuned Assistant Checkpoints**: Supervised fine-tuning for structured tool calling, database querying, and strict factual compliance.
- 🎧 **Adaptive Hardware Echo Cancellation**: Automated acoustic echo suppression for live speakerphone and open microphone deployments.
- 💬 **Dynamic Emotion & Prosody Sliders**: Fine-grained runtime control over pitch inflection, speaking tempo, and emotional intensity.

---

### 🔍 Related Search Tags
`haru 4b` • `vibevoice` • `elevenlabs alternative` • `haru ai` • `voice cloning ai` • `speech to speech ai` • `speech to speech` • `open source voice` • `realtime voice ai` • `voice to voice` • `ai voice bot` • `open source speech model` • `haru streaming` • `local speech ai` • `whisper alternative` • `multilingual voice ai` • `offline voice agent` • `haru-4b` • `zero shot voice cloning` • `instant voice clone` • `realtime speech ai` • `qwen3.5 4b` • `tts alternative` • `real time translation` • `speech streaming` • `local voice ai` • `streaming voice ai`

