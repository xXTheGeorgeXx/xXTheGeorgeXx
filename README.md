# Jorge Luis Rodríguez Andino

Systems Engineering student (4th year) from Paraguay, working on **Edge AI**: running large language models locally on everyday phones — no cloud, no API keys, no subscription.

*Soy de Paraguay y trabajo en IA local: modelos que corren en el teléfono, sin nube.*

## Modula — custom llama.cpp engine for Android

My main project. A custom-built `llama.cpp` inference engine (JNI) for ARM64 Android, CPU-only:

- Gold-core CPU affinity, Q8_0 KV cache, streaming generation with a sliding-window context and UTF-8-safe token callbacks
- Runs **Gemma 4 E2B (IQ4_NL)** fully offline on a Samsung Galaxy A52 (6 GB RAM, Snapdragon 720G, CPU only)
- Verified on the phone, 2026-11-06: a 2,170-token answer in 391.6 s at **5.54 tok/s** (TTFT 1.38 s, context 2,208 / 8,192 tokens); short replies at 3.4–3.5 tok/s
- Test APK (8.5 MB) with the stripped engine (`libmodula_engine.so`, 6.7 MB) + `libomp.so`

Repo: [ModulaApp](https://github.com/xXTheGeorgeXx/ModulaApp)

## ExamSaaS v5 — in progress

A free SaaS for teachers: teachers manage exams from a control panel, students take them with their ID number via a link, and get a PDF with a partial score. Currently in development and not yet published on GitHub.

## How I work now

I don't write code line by line anymore. I bring the idea and the architecture, and I direct AI agents to do the heavy implementation — then I test the result on real hardware, on my own phone.

- Idea and system architecture: modular design, low-cost Edge AI, RAG engines, SaaS platforms, database normalization
- AI-assisted development: I direct agents, review what they build, and verify it running locally
- On-device testing: Termux, Android, quantized models on limited hardware

## Stack

llama.cpp · GGUF · Android NDK · Termux · Supabase · RAG · Modular architecture

## Contact

- GitHub: [@xXTheGeorgeXx](https://github.com/xXTheGeorgeXx)
