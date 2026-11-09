<p align="center">
  <img width="112" height="112" alt="Oxide" src="https://raw.githubusercontent.com/getoxide/oxide/main/assets/brand/oxide/png/avatar/512x512.png" />
</p>

<h1 align="center">Oxide</h1>

<p align="center">
  <strong>Open-source tools for agentic engineering.</strong><br />
  We build for the end of the agent loop: reviewing what coding agents wrote, proving what was actually checked, and merging with confidence.
</p>

<p align="center">
  <a href="https://github.com/getoxide/oxide/actions/workflows/ci.yml"><img alt="CI" src="https://github.com/getoxide/oxide/actions/workflows/ci.yml/badge.svg?branch=main" /></a>
  <a href="https://github.com/getoxide/oxide/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
  <img alt="Platforms: macOS and Windows" src="https://img.shields.io/badge/platform-macOS%20%7C%20Windows-lightgrey.svg" />
  <img alt="Status: pre-release" src="https://img.shields.io/badge/status-pre--release-yellow.svg" />
</p>

<p align="center">
  <a href="https://github.com/getoxide/oxide">Oxide</a> ·
  <a href="https://github.com/getoxide/oxide/releases">Releases</a> ·
  <a href="https://github.com/getoxide/oxide/blob/main/CONTRIBUTING.md">Contributing</a> ·
  <a href="https://github.com/getoxide/oxide/blob/main/SUPPORT.md">Support</a> ·
  <a href="https://github.com/getoxide/oxide/blob/main/LICENSE">MIT License</a>
</p>

---

## What we build

**[Oxide](https://github.com/getoxide/oxide)** is a free, open-source desktop app for reviewing and merging what your coding agents write. It drives **Claude Code**, **OpenAI Codex** and **Antigravity CLI** from one window, with Git, GitHub, a code editor and a terminal around the conversation.

It doesn't ship an agent of its own, and no code or prompt goes through a server of ours: the CLIs you already have installed and logged in do the work, and Oxide shows exactly what came back.

| Review before you merge | One window, every agent | Local by default |
| :-- | :-- | :-- |
| Per-Turn, Uncommitted and Branch diffs backed by Checkpoints. A Verification Dossier says which checks ran, what stayed unverified and which risk signals fired — separate facts, never a single score. | Native adapters for Claude Code, Codex and Antigravity CLI behind one Thread, Model, Effort and Permission mode. Slash commands, skills, attachments and usage limits included. | Threads, Transcripts and Checkpoints stay in a local SQLite database. No telemetry. Dictation runs fully on-device. Your code goes only to the Provider you chose. |

## What's inside

- **Diffs by Turn.** A Checkpoint at the start and end of every Turn shows exactly what that Turn changed, with line comments you can send back as one prompt or submit as a GitHub review.
- **Blind review.** A second Provider reviews the diff and the issue, never the original conversation. Its findings become comments you keep or dismiss.
- **Revert and Restore.** Remove one hunk or put a Thread's files back to how they were before any Turn. Both are undoable.
- **Git and GitHub.** Branches, commit and push, pull requests with checks and inline threads, and Issues, through `git` and the GitHub CLI.
- **A workspace, not a chat box.** Monaco with language servers for Rust, TypeScript/JavaScript, Python and C/C++, per-Project terminals, and an Attention Center for every Thread waiting on you.
- **Rust and Tauri 2.** A native Core owns files and processes; the webview gets no filesystem or shell permission.

## Get started

Download the installer for **macOS (Apple Silicon)** or **Windows x64** from [Releases](https://github.com/getoxide/oxide/releases), or build from source. You need at least one Provider installed and logged in, plus `git`; the GitHub CLI is optional and enables the pull request and Issues features.

> [!NOTE]
> Oxide is pre-release software. Expect rough edges and breaking changes between versions.

## Built in the open

Contributions are welcome. Start with [CONTRIBUTING.md](https://github.com/getoxide/oxide/blob/main/CONTRIBUTING.md) for the trunk-based branch model, local checks and pull request conventions, and look for [`good first issue`](https://github.com/getoxide/oxide/issues?q=is%3Aissue%20is%3Aopen%20label%3A%22good%20first%20issue%22) or [`help wanted`](https://github.com/getoxide/oxide/issues?q=is%3Aissue%20is%3Aopen%20label%3A%22help%20wanted%22).

Oxide is MIT-licensed. The [domain language](https://github.com/getoxide/oxide/blob/main/GLOSSARY.md) and every [architecture decision](https://github.com/getoxide/oxide/tree/main/docs/adr) are written down in the repository.

---

<p align="center">
  <sub>Claude Code, Codex and Antigravity are trademarks of their respective owners. Oxide is an independent project, not affiliated with or endorsed by Anthropic, OpenAI or Google.</sub>
</p>
