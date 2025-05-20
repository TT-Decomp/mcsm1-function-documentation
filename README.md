# 🧠 MCSM1 Function Documentation

This repository contains detailed notes and labels for function offsets found within **Minecraft: Story Mode – Season 1 Complete Edition**.  
It is part of the broader effort under the [TT-Decomp](https://github.com/TT-Decomp) organization to reverse-engineer and document the Telltale Tool engine.

---

## 📘 Purpose

The goal of this repo is to maintain a centralized, human-readable reference of:

- Function **offsets** in the game binary
- **User-assigned names** based on behavior
- **Guessed purpose** or role in the engine/system

All labels are inferred through reverse engineering (e.g., IDA, Ghidra) and may evolve as analysis progresses.

---

## 🗂 Structure

Function entries are stored in this format:

| Offset     | Name             | Description / Guess                                     |
|------------|------------------|----------------------------------------------------------|
| `0x1ECAC0` | `TT_LogShutdown` | Called during system shutdown; logs source file strings |
| `0x14F8A0` | `SceneManager::Init` | Likely related to scene system initialization         |
| ...        | ...              | ...                                                      |

You can find the full list in [`FUNCTIONS.md`](FUNCTIONS.md).

---

## 📎 Conventions

- Offsets are in **hex**, relative to the main executable base.
- Names are **user-defined** and follow C++-style conventions when applicable.
- Descriptions are based on behavior, naming clues, and reverse engineering context.
- If the purpose is unclear, use `???` and update when more is known.

---

## 📬 Contributions

Found and identified a function? Open a PR or submit an issue using this format:

```txt
Offset: 0x123456
Suggested Name: ActorComponent::Update
Guess of Purpose: Runs every frame to update actor logic.
````

All contributors will be credited in the project and in `CREDITS.md`.

---

## 📌 Disclaimer

This project is for **educational and preservation** purposes only.
We do not distribute game files or any copyrighted material.

