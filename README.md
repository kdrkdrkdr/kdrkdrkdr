<h1 align="left">Hi 👋, I'm Gyeongmin Kim (kdr)</h1>

I optimize AI models — LLM · TTS · ASR · voice conversion · speech enhancement — tearing models apart (quantization, SIMD, speculative decoding, pure-C rewrites) and building the serving around them so they run in production.

- 🤗 [Hugging Face](https://huggingface.co/kdrkdrkdr)
- 💼 [LinkedIn](https://www.linkedin.com/in/kdrkdrkdr)
- 📫 kdrkdrkdr@hanyang.ac.kr

---

## 📝 Publications

**Preprints**

- **faster-enhancer.c: A Dependency-Free int8 Runtime for Streaming Speech Enhancement on Commodity CPUs**
  **Gyeongmin Kim.** arXiv:2607.25350, Jul 2026.
  [[arXiv]](https://arxiv.org/abs/2607.25350) [[code]](https://github.com/kdrkdrkdr/faster-enhancer.c)
- **Extracting Voice Styles from Frozen TTS Models via Gradient-Based Inverse Optimization**
  **Gyeongmin Kim.** arXiv:2607.25351, Jul 2026.
  [[arXiv]](https://arxiv.org/abs/2607.25351) [[code]](https://github.com/kdrkdrkdr/supertonic.embed)

**Under review**

- **Why One Small Fixed Tree Suffices: The Cost Geometry of Draft Trees for a Multi-Token-Prediction Drafter**
  **Gyeongmin Kim**, Ayoung Moon, Seung Jin Lee. Under review, 2026.

## 💼 Experience

- **NC AI** *(Seongnam, South Korea)* — Data Engineering Team *(May 2026 – )*
  LLM inference optimization & serving — MoE quantization (W8A16), speculative decoding for a data-generation pipeline, and a distributed vLLM serving gateway in Go.
- **Yonsei University Health System (YUHS)** *(Seoul, South Korea)* — Research Engineer *(Mar 2025 – Oct 2025)*
  Led dev for NGS clinical report pipeline & SICU false-alarm monitoring desktop app.
- **NCSOFT** *(Seongnam, South Korea)* — Audio Data Team *(Jul 2024 – Jan 2025)*
  Built end-to-end audio post-processing automation for TTS data pipelines.
- **Taiyaki Studios** *(USA, Remote)* — AI Team *(Jan 2023 – Jul 2023)*
  Built a complete TTS training toolkit and production inference pipeline.

## 🚀 Personal Projects

**Model Optimization (Nov 2024 – present)** — speech models re-implemented in dependency-free pure C, running in real time on-device
- [**nemotron-asr-streaming.c**](https://github.com/kdrkdrkdr/nemotron-asr-streaming.c) — 0.6B streaming ASR (FastConformer + RNN-T). Cache-aware streaming, W8A8 quantization with custom "Q8P" 4-row tile packing, NEON/AVX2 SIMD, up to 16 threads. [[docs]](https://github.com/kdrkdrkdr/nemotron-asr-streaming.c/blob/w8a8/MODEL.md) [[quantized model]](https://huggingface.co/kdrkdrkdr/nemotron-3.5-asr-streaming-0.6b-w8a8)
- [**LILAC**](https://github.com/kdrkdrkdr/lilac) — Zero-shot real-time voice conversion from a 3s reference (OpenVoice v2 port). Streaming HiFi-GAN decoder, 2-thread SPSC audio pipeline, RNNoise SIMD. RTF 0.7–0.8 on CPU, 270–330 ms end-to-end. [[optimizations]](https://github.com/kdrkdrkdr/lilac/blob/main/Optimization.md)
- [**MossTTS-Nano.c**](https://github.com/kdrkdrkdr/MossTTS-Nano.c) — 100M TTS model. NEON/SSE SIMD, KV cache, pthread parallelism — **30× speedup** (68s → 2.3s), 1.8× faster than PyTorch CPU, RTF 0.33. [[optimizations]](https://github.com/kdrkdrkdr/MossTTS-Nano.c#optimizations-applied)
- [**DeepFilterNet3.c.wasm**](https://github.com/kdrkdrkdr/DeepFilterNet3.c.wasm) — Noise-reduction model in pure C/WASM, real-time in mobile browsers. ~1 ms/frame on MacBook M2, ~4 ms on Galaxy S23. [[optimizations]](https://github.com/kdrkdrkdr/DeepFilterNet3.c.wasm/blob/main/OPTIMIZATION.md)

**[Axcellworks](https://www.axcellworks.com) (JP) — real-time voice conversion intelligibility, remote collaboration (Nov 2023 – Feb 2024)**
- Diagnosed chunk-boundary artifacts as receptive-field truncation; removed them with overlap-save chunk inference (neighbor-chunk context, keep center) at no added latency.

**Multilingual TTS (Oct 2022 – Feb 2025)**
- Data — BGM removal (Kim Vocal) → speaker diarization (pyannote) → VAD segmentation → Whisper transcription: ~30k clips (3–10 s).
- Models — VITS derivatives: [**JA2ML-VITS**](https://github.com/kdrkdrkdr/JA2ML-VITS) (19-language speech from Japanese-only data), [**JK-VITS**](https://github.com/kdrkdrkdr/JK-VITS) (KO/JA bilingual), [**RVC-VITS**](https://github.com/kdrkdrkdr/RVC-VITS) (RVC-converted training data).
- Services — [**ProsekaTTS**](https://huggingface.co/spaces/kdrkdrkdr/ProsekaTTS) (**2.3M+ visitors, 60 developer duplicates**, Jul 2026) · [**ShirokoTTS**](https://huggingface.co/spaces/kdrkdrkdr/ShirokoTTS) (EN/KO/JA).

**G2P Packages (Jun 2023 – Dec 2023)**
- [**g2pk3**](https://github.com/kdrkdrkdr/g2pk3) — Korean/Japanese/English → Korean pronunciation. [[PyPI]](https://pypi.org/project/g2pk3/)
- [**ko2kana**](https://github.com/kdrkdrkdr/ko2kana) — Korean/English pronunciation → Katakana. [[PyPI]](https://pypi.org/project/ko2kana/)

**Japanese Translation Tools (Dec 2020 – Apr 2022)**
- [**novel-reader**](https://github.com/kdrkdrkdr/novel_reader) — Android app translating novels from 7 Japanese sites with a proper-noun dictionary system.
- [**EhndWebTranslate**](https://github.com/kdrkdrkdr/EhndWebTranslate) — Async Japanese web page translator with real-time/document/novel modes.
- [**UserDict4Papago**](https://github.com/kdrkdrkdr/UserDict4Papago) — Proper-noun dictionary overlay for Papago KR-JP translation.

## 🌱 El Nino (Apr 2024 – Apr 2026)

Founded [**El Nino**](https://elnino.kr) (university startup club → sole proprietorship) and built **Knoc**, a real-time translation subtitle service for classes and conferences — launched Mar 2026, covered by [Multilingual.com](https://multilingual.com/elnino-launches-knoc-ai-subtitle-solution-multilingual-communication/).

- Rewrote the Python prototype in Go for large-scale WebSocket handling; Redis Pub/Sub subtitle rooms, distributed architecture, user/admin dashboards with PAYG & subscription billing.
- Knoc-Overlay desktop subtitle overlay (Electron) · [elnino.kr](https://elnino.kr) website.
- Selected for MOE U300+ student startup track (2024) · served Konkuk Univ. winter school & KSRT conference.

## 🎓 Education

- [**Hanyang University**](http://cs.hanyang.ac.kr/), Seoul, South Korea — B.S. in Computer Science *(Mar 2023 – Present, Leave of Absence since Jul 2024)*
