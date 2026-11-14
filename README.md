<div align="center">

# Clip Atlas

**Every clip, mapped to its game.**

A native OBS Studio plugin that files your replays, recordings and screenshots into per-game folders, automatically.

[Download](https://github.com/sxnfer/clip-atlas/releases/latest) · [Install guide](docs/install.md) · [Features](docs/features.md) · [Changelog](CHANGELOG.md)

<br>

<img src="docs/activity-preview/dark-expanded.png" width="420" alt="The activity pill sorting a Counter-Strike 2 replay">

</div>

<br>

| | |
| --- | --- |
| **Finds the game** | Watches your Game and Window Capture sources. Nothing to configure. |
| **Sorts every save** | Replays, recordings (split parts included) and screenshots. |
| **Runs the Replay Buffer** | Starts when a game starts, stops when it closes. |
| **Browses your clips** | A dock with thumbnails, search, filters, rename and move. |
| **Never loses a file** | Moves are verified; nothing is ever deleted for good. |
| **Updates itself** | Installs the new version when you close OBS. |

```
Clips/
├── Counter-Strike 2/
│   └── 2026-10/
│       └── Replay 2026-10-23 19-02-44.mkv
├── Elden Ring/
└── Unsorted/
```

Windows 10 or 11 · OBS Studio 31+ · 64-bit

## Develop

Core logic is plain C++17, unit-tested without OBS:

```sh
cmake -S tests -B build/tests && cmake --build build/tests && ctest --test-dir build/tests --output-on-failure
```

<sub>Replaces the original Python script, kept in <a href="legacy/">legacy/</a>. Roadmap: <a href="docs/PLAN.md">docs/PLAN.md</a></sub>
