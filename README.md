# Homebrew tap for squish

[Squish](https://github.com/konjoai/squish) — local LLM inference server for
Apple Silicon with block-level paged KV cache, INT3 support, and an
OpenAI-compatible API.

## Install

```bash
brew tap konjoai/squish
brew install squish
```

## Update

```bash
brew update
brew upgrade squish
```

## Requirements

- macOS 13+ on Apple Silicon (M1–M5). The formula refuses to install on
  Intel because `mlx` is Apple-Silicon-only.
- Python 3.12 (installed automatically as a Homebrew dependency).

## What you get

After `brew install squish`, four CLI entry points are on your `PATH`:

| Command | Purpose |
|---|---|
| `squish` | Main CLI (`squish run`, `squish pull`, `squish serve`, …) |
| `squish-server` | Standalone FastAPI server entry point |
| `squish-convert` | One-shot model conversion utility |
| `squishd` | Persistent daemon with UDS IPC |

The PyPI distribution is `squish-ai`; the installed Python module and CLI
are both `squish`.

## Issues

Report formula issues here. Report squish bugs at
[konjoai/squish](https://github.com/konjoai/squish/issues).
