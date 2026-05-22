<h1 align="left">Hi 👋, I'm Gyeongmin Kim (kdr)</h1>

Software engineer working on **speech processing**, **on-device model optimization**, and **real-time audio systems**.
Co-founder of [**El Nino**](https://elnino.kr), building [**Knoc**](https://elnino.kr) — a real-time translation subtitle service.

- 📄 [Portfolio / CV](https://kdrkdrkdr.github.io/)
- 🏢 [Team El Nino](https://elnino.kr)
- 🤗 [Hugging Face](https://huggingface.co/kdrkdrkdr)
- 📫 kdrkdrkdr@hanyang.ac.kr

---

## 📝 Publications

- **Extracting Voice Styles from Frozen TTS Models via Gradient-Based Inverse Optimization**
  *Gyeongmin Kim.* Preprint, Apr 2026. *To be submitted to ICASSP 2027 / Interspeech 2027.*
  [[DOI]](https://doi.org/10.5281/zenodo.19646514) [[supertonic.embed]](https://github.com/kdrkdrkdr/supertonic.embed) [[kokoro.embed]](https://github.com/kdrkdrkdr/kokoro.embed)

## 💼 Experience
- **NC AI** *(Seongnam, South Korea)* — Data Engineer, Contract *(May 2026 – )*
  Data Engineering and Model Optimization for Multimodal AI Training/Inference
- **Yonsei University Health System (YUHS)** *(Seoul, South Korea)* — Research Engineer *(Mar 2025 – Oct 2025)*
  Led dev for NGS clinical report pipeline & SICU false-alarm monitoring desktop app.
- **NCSOFT** *(Seongnam, South Korea)* — Audio Data Engineer, Contract *(Jul 2024 – Jan 2025)*
  Built end-to-end audio post-processing automation for TTS data pipelines.
- **Axcellworks** *(Japan, Remote)* — Speech Engineer, Freelance *(Nov 2023 – Feb 2024)*
  Improved real-time Voice Changer intelligibility via chunk merging algorithm.
- **Taiyaki Studios** *(USA, Remote)* — AI Engineer, Contract *(Jan 2023 – Jul 2023)*
  Built a complete TTS training toolkit and production inference pipeline.

## 🚀 Featured Projects

**On-Device Speech Model Optimization (C / WebAssembly)**
- [**MossTTS-Nano.c**](https://github.com/kdrkdrkdr/MossTTS-Nano.c) — 100M TTS model rewritten in pure C. NEON/SSE SIMD, KV cache, pthread parallelism — **30× speedup** (68s → 2.3s), **1.8× faster than PyTorch CPU**, RTF 0.33.
- [**DeepFilterNet3.c.wasm**](https://github.com/kdrkdrkdr/DeepFilterNet3.c.wasm) — Noise-reduction model in pure C/WASM. ~1 ms on MacBook M2, ~4 ms on Galaxy S23.
- [**fastenhancer.c.wasm**](https://github.com/kdrkdrkdr/fastenhancer.c.wasm) — Audio enhancement in pure C. **546× size reduction** (183 KB), mobile RTF 0.28.
- [**LILAC**](https://github.com/kdrkdrkdr/lilac) — Zero-shot real-time voice conversion from 3s audio. OpenVoice v2 ported from PyTorch to pure C with streaming HiFi-GAN decoder, RNNoise SIMD, 2-thread SPSC audio pipeline. RTF 0.7–0.8 on CPU.

**Multilingual TTS & Voice Conversion**
- [**JA2ML-VITS**](https://github.com/kdrkdrkdr/JA2ML-VITS) — Multilingual TTS inducing 19-language speech from Japanese-only datasets.
- [**JK-VITS**](https://github.com/kdrkdrkdr/JK-VITS) — Korean/Japanese bilingual TTS.
- [**RVC-VITS**](https://github.com/kdrkdrkdr/RVC-VITS) — Voice-conversion-based dataset augmentation and TTS training pipeline using RVC.
- [**ProsekaTTS**](https://huggingface.co/spaces/kdrkdrkdr/ProsekaTTS) — Character TTS service. **2.1M+ visitors** (Feb 2026).
- [**ShirokoTTS**](https://huggingface.co/spaces/kdrkdrkdr/ShirokoTTS) — First-ever Blue Archive Shiroko TTS.

**G2P Packages (PyPI)**
- [**g2pk3**](https://pypi.org/project/g2pk3/) — Korean/Japanese/English → Korean pronunciation.
- [**ko2kana**](https://pypi.org/project/ko2kana/) — Korean/English pronunciation → Katakana.

**Japanese Translation Tools**
- [**novel-reader**](https://github.com/kdrkdrkdr/novel_reader) — Android app translating novels from 7 Japanese sites with a custom proper-noun dictionary system.
- [**EhndWebTranslate**](https://github.com/kdrkdrkdr/EhndWebTranslate) — Async Japanese web page translator with real-time/document/novel modes.
- [**UserDict4Papago**](https://github.com/kdrkdrkdr/UserDict4Papago) — Proper-noun dictionary overlay for Papago KR-JP translation.

## 🌐 Open Source Contributions

- [**VOICEVOX Engine**](https://github.com/VOICEVOX/voicevox_engine) — Added Korean speech support by mapping Japanese phonemes to Korean phonemes.
- [**Versatile Audio Super Resolution**](https://github.com/haoheliu/versatile_audio_super_resolution) — Contributed silence-removal utility for upsampled audio.
- [**Manga Image Translator**](https://github.com/zyddnys/manga-image-translator) — Maintained translation module for image translation web service.

## 🎓 Education

- [**Hanyang University**](http://cs.hanyang.ac.kr/), Seoul, South Korea — B.S. in Computer Science *(Mar 2023 – Present, Leave of Absence since Jul 2024)*
