# PolyTrack AI

An unofficial educational AI project that teaches a software agent to drive [PolyTrack](https://app.polytrack.kodub.com/), a low-poly browser-based racing game by Kodub.

> **Status:** Early development. This README will be updated as the project progresses.

## What it is

A personal computer-science / AI portfolio project. The goal is to build a learned agent that drives PolyTrack from screen pixels:

1. **Imitation learning baseline** — record human gameplay, then train a CNN to predict driving inputs from frames.
2. **Reinforcement learning extension** — warm-start from the IL model, then improve through trial and error using a reward signal extracted from the screen.

The agent perceives the game purely through screen capture and acts on the game purely through emulated keyboard input — the same channels available to any human player.

## What it isn't

This project is **not affiliated with, endorsed by, or sponsored by** Kodub or the PolyTrack team. It does not modify the game, read its memory, interfere with online play, or submit anything to leaderboards. See [DISCLAIMER.md](DISCLAIMER.md).

## Roadmap

- [ ] Game interface — screen capture + keyboard input
- [ ] Data collection — record human gameplay
- [ ] Imitation learning baseline
- [ ] Live driving — trained agent attempts the game
- [ ] Evaluation and analysis
- [ ] Public polish (this README, demo, writeup)
- [ ] Reinforcement learning extension

Detailed progress, demos, and results will land here as each milestone ships.

## Tech stack (planned)

- Python 3.11+
- PyTorch
- `mss` for screen capture, `pydirectinput` for keyboard input
- OpenCV / NumPy for image work
- Stable-Baselines3 + Gymnasium for the RL extension

---

This project is for personal learning and educational purposes. Please support the [original game](https://app.polytrack.kodub.com/) and its creators.
