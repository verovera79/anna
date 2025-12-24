# TikTok Cover Generation — Strict Codex

This repository contains a strict, self-controlling protocol for generating
TikTok / Reels / Shorts news covers in a fully automated and reproducible way.

The system is designed for media use cases where:
- text must be rendered 1:1 without any modification
- visual style must remain consistent across large volumes
- no clarification, confirmation, or interpretation is allowed
- automation and repeatability are critical

## Core Concept

The workflow is based on a strict separation of responsibilities:

- DALL·E generates ONLY the background image (no text)
- ChatGPT Canvas overlays the text EXACTLY as provided
- The input phrase is treated as immutable data

## How It Is Used

1. The user provides:
   - one source image
   - one source text phrase (raw, unedited)

2. The CODEX protocol is applied verbatim.
3. The result is a ready-to-publish 9:16 cover image.

The CODEX.md file defines all mandatory rules and prohibitions.
No improvisation or creative interpretation is allowed.

## Important

This repository is a protocol storage.
The CODEX is manually or programmatically injected into ChatGPT
during generation. It is NOT automatically applied by GitHub.

For actual rules, see: CODEX.md
