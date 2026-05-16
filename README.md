# Hola, soy Héctor Martínez

Desarrollador Full-Stack de Querétaro, México. Actualmente construyendo **LifeOS / Axi**.

## Qué es LifeOS / Axi

Un asistente personal de IA **local-first** que vive en mi laptop. No es servicio en la nube ni dependencia de un vendor — corre 100% en mi propio hardware, escucha por el micrófono, ve mi pantalla y mi cámara, traduce videos en tiempo real, graba reuniones, y recuerda lo que pasó.

No es solo una idea — es un sistema real que uso todos los días.

### Lo que ya funciona hoy

- 🎤 **Voz (Axi)**: dictado, preguntas con pantalla, preguntas con cámara. Whisper turbo en GPU + Piper TTS en español mexicano. Comandos de voz tipo "Axi, abre el dashboard"
- 🧠 **Cerebro**: Qwen3.6 35B-A3B (MoE) corriendo en 12 GB de VRAM vía llama.cpp. Selector de modelos con catálogo de 9 multimodales 2026 (Qwen3.5, Qwen3.6, Gemma 4, Nemotron 3 Omni) y editor de parámetros por modelo desde el dashboard
- 🎙️ **Reuniones**: grabador de reuniones largas con transcripción incremental, diarización de hablantes (Resemblyzer + pyannote opt-in), screenshots con dedup, resúmenes generados por Qwen
- 🧩 **Memoria**: SQLite + FTS5 con historial de conversaciones, extracción de hechos, búsqueda full-text, timezone-aware
- 🌐 **Intérprete EN→ES en tiempo real**: Whisper streaming + Qwen + Piper. Captura el audio del sistema vía PipeWire null-sink. Sub-3s de latencia
- 🎮 **Game Guard**: libera los 12 GB de VRAM con un click para juegos exigentes. Después restaura todo
- 📊 **Dashboard observable**: FastAPI + Alpine.js + Tailwind. Event log, métricas de latencia del brain (p50/p95), daily digest, búsqueda en reuniones, selector de modelos
- 🔔 **Tray KDE**: indicador de estado, comandos rápidos, tooltip con ubicación de modelos en GPU/RAM
- ✅ **241 tests passing**, observabilidad real (no más "se cayó algo silenciosamente")

## Stack principal

**LifeOS / Axi:** Python 3.12, FastAPI, SQLite + FTS5, llama.cpp, faster-whisper, Piper, PipeWire, KDE Plasma, systemd, pytest

**Hardware target:** RTX 5070 Ti Laptop (12 GB VRAM, Blackwell sm_120), CachyOS / Arch / Fedora Linux

**Web / Freelance:** Next.js, NestJS, PostgreSQL, Docker, n8n, TypeScript

## Proyectos

| Proyecto | Descripción | Stack |
|---|---|---|
| [LifeOS / Axi](https://github.com/hectormr206/lifeos) | Asistente de IA local-first | Python, llama.cpp, FastAPI |
| [lifeos-site](https://github.com/hectormr206/lifeos-site) | Landing page de LifeOS | React 19, Vite, Tailwind |

## Filosofía

- **Local-first** — nada va a la nube por default
- **Privacy by default** — audio, conversaciones y reuniones se quedan en disco propio
- **Single user, single laptop** — no multi-tenant, no auth, no cloud sync
- **AI is a tool** — nosotros dirigimos, la AI ejecuta. El humano siempre lidera

## Contacto

- 🌐 Web: [hectormr.com](https://hectormr.com)
- 🚀 LifeOS: [lifeos.hectormr.com](https://lifeos.hectormr.com)
- 💼 LinkedIn: [hectormr206](https://linkedin.com/in/hectormr206)
