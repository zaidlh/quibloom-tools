# Quibloom Quiz Video Tools

Renderer and production toolkit for full-length vertical quiz videos
(about 6 minutes, 15 questions each): animated option cards synced to
narration, a 5-second countdown, and a green answer reveal.

Start with [SKILL.md](SKILL.md): the full production recipe, from question
format through voice production, rendering, QA, and publishing metadata.
Arabic summary: [README.ar.md](README.ar.md).

## What is included

- `renderer/`: the video builder, QA and finishing scripts
- `SKILL.md`: the production recipe
- `docs/PRODUCTION-SPEC.md`: the pipeline specification
- `assets/quibloom-logo.png`: the brand logo

Question banks and voice clips are not included. Section 3 of SKILL.md
describes the question JSON format so you can write your own.

## Quick start

Requirements: Python 3.9+, `pip install pillow numpy`, ffmpeg with libx264,
and Noto Sans fonts (`apt install fonts-noto-core` on Debian/Ubuntu).

```bash
python3 renderer/main2.py YOUR_VIDEO.json CLIPDIR out.mp4
```

`CLIPDIR` is a folder of WAV clips named as in SKILL.md section 4.

## License

- **Code and tools** (everything in this repository): MIT License. See
  [LICENSE](LICENSE).
- **Brand** (the Quibloom name and logo): not covered by the MIT License.
  Forks may not use the name or logo to imply endorsement without permission.
- **Question banks**: not part of this repository. They are sold separately
  under their own commercial license.
- **Fonts**: Noto Sans is licensed under the SIL Open Font License.
