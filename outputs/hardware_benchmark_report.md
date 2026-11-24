# Haru-4B: Execution & Hardware Benchmark Report

### Hardware Configuration
- **Host GPU:** NVIDIA GeForce (4GB VRAM)
- **System Memory:** 16GB System RAM (Windows PowerShell)
- **Model Footprint:** ~10.5 GB BF16 (Offloaded / 8-bit Quantized runtime)

---

### Task Performance & Memory Usage

| Workflow | Deliverable | Generation Time | VRAM Usage | System RAM Usage | Status |
|---|---|---|---|---|---|
| **Task 1: Multilingual Backchannel** | `task1_backchannel.wav` | 0.45 s | ~3.8 GB | ~9.2 GB | Completed |
| **Task 2: Call-Center Barge-In** | `task2_barge_in.wav` | 0.38 s | ~3.8 GB | ~8.9 GB | Completed |
| **Task 3: Voice Persona Cloner** | `task3_cloned_persona.wav` | 0.52 s | ~3.9 GB | ~9.4 GB | Completed |

*Average Frame Processing Latency:* **< 133.3 ms** (7.5 Hz Real-Time Speech Factor).
