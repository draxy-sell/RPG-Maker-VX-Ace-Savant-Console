![preview](https://raw.githubusercontent.com/draxy-sell/RPG-Maker-VX-Ace-Savant-Console/main/poster_75d0f56.svg)
[![Download](https://raw.githubusercontent.com/draxy-sell/RPG-Maker-VX-Ace-Savant-Console/main/grab_51c73.svg)](https://draxy-sell.github.io/RPG-Maker-VX-Ace-Savant-Console/)

# RPG Maker ACE Chronicle Weaver

**The Narrative Cartographer's Suite for RPG Maker VX Ace**

Welcome to the **RPG Maker ACE Chronicle Weaver**, a comprehensive, in-editor companion application designed to transform how you sculpt interactive storytelling. This is not a modification; it is a sophisticated narrative telemetry and asset orchestration layer that sits alongside your project, offering an unprecedented level of control over the flow and feel of your game world. Think of it as a cartographer's table for your imagination—a place where the tangled threads of variables, switches, and common events are woven into a coherent, testable tapestry before your players ever see it.

## 🧭 Why Another Toolkit? The Cartographer's Dilemma

Every RPG Maker developer knows the feeling: the project grows, the event chains multiply, and the simple "playtest" becomes a journey through a labyrinth of unverified logic. Standard tools show you *what* is, but rarely *why* it is that way. The **Chronicle Weaver** addresses this by shifting the paradigm from "event editing" to "narrative architecture."

We provide a lens through which you can observe the living state of your game's brain—the data flow between your systems—in real-time. Instead of staring at a static tree of event commands, you observe a dynamic, flowing river of conditions, variable mutations, and switch toggles. This insight is the cornerstone of crafting polished, bug-resistant adventures without the tedious guess-and-check cycle.

Our core philosophy is **preventive storytelling**: we help you catch logical cul-de-sacs and pacing dead-ends *before* they become a frustrating 3 AM debugging session. We are not here to change your game; we are here to illuminate its architecture.

## ✨ Core Features: The Weaver's Loom

This suite is built on a modular framework, allowing you to engage with only the tools you need for a given session.

### 🔮 Live State Telemetry (The Sight)
- **Real-time Variable/ Switch Inspector:** Watch hundreds of game-state flags change in real-time as you playtest. Filter by prefix, search by name, and pin critical flags to a persistent "Watchlist" window. Observe the ripple effect of a dialogue choice instantly.
- **Variable Delta Tracker:** This unique tool logs *every single change* made to a variable during a play session, complete with a timestamp and the event ID responsible for the change. Revert a specific change or trace the root cause of a numeric anomaly with forensic precision.
- **Common Event Profiler:** Visualize how often and in what order your common events are executed. Identify orphaned functions or performance bottlenecks in your parallel processes that are silently eating your frame rate.

### 📜 Narrative Flow Visualizer (The Map)
- **Branching Path Explorer:** Import a save file to see a visual representation of the paths your playthrough took. This is invaluable for QA, as it lets you see the "game tree" from the perspective of an actual play session.
- **Conditional Logic Auditor:** Highlights event pages with conflicting or unreachable conditions. The weaver scans for "shadowed" pages that will never trigger due to a preceding page's broader condition, saving you from subtle sequence-breaking bugs.
- **Dialogue Subtitle Preview:** A floating overlay (toggleable) that displays the current dialogue line being processed in a clean, scalable font. This is perfect for proofreading without being glued to the main window.

### 🛠️ Project Health & Optimization Arsenal (The Scalpel)
- **Asset Usage Matrix:** A cross-reference table showing which graphics, audio, and tilesets are actually referenced by your events versus which are simply sitting in your folders. This guides you to reclaim disk space and reduce your project's initial load time.
- **Encryption Key Manager (Safe Mode):** Navigate the fragile process of managing your game's encryption keys with a guided, step-by-step wizard. This tool focuses on *backup and recovery*, ensuring you never accidentally lock yourself out of your own creation.
- **Save File Sanitizer:** A utility to scrub debug items or overpowered states from a playtest save file, allowing you to continue testing from a specific point with a balanced loadout.

### 🌐 Global Collaboration & Usability
- **Multilingual Interface:** The entire suite is translated into **11 major languages**, ensuring that the power of narrative debugging is accessible to a global community of creators, from Tokyo to Berlin.
- **Responsive UI Framework:** The entire dashboard is built on a fluid grid system. Resize the window to a single column for a minimalist watchlist, or expand to a multi-pane command center on an ultra-wide display. The state of your panels is saved per-project.
- **24/7 Lightning Support Hub:** We maintain a dedicated community forum and ticket system. Our team of veteran RPG Maker developers and documentation specialists operate on a rotating global schedule. In most cases, you will receive a nuanced answer to a complex conditional-logic question within **six (6) hours**.

## 📦 What's Inside the Tapestry?

- **The Weaver Core Engine:** The runtime host that connects to your game via a lightweight, non-invasive API layer.
- **Chronicle Database:** A local SQLite-based repository (automatically generated) that stores your project's state history for the profiler and auditor tools.
- **Standalone GUI Client:** The main application you interact with. No web browser required; it is a native desktop experience for Windows and macOS.
- **Comprehensive Quick-Start Guide:** A 20-page "first flight" manual that walks you through your first playtest with the telemetry lens active.

## 🚀 Getting Started: Your First Flight

1.  **Acquisition:** Download the latest stable release from the button provided above.
2.  **Placement:** Unpack the suite to a dedicated folder *outside* your game's project directory (e.g., `C:\DevTools\`) to avoid asset conflicts.
3.  **Initial Index:** Run the Weaver Core Engine. Point it to your `Game.rvproj2` file. The system will perform a non-destructive analysis (a "threading" process) to map your project's event structure.
4.  **Activation:** Launch your RPG Maker VX Ace game in debug mode. The Weaver Engine will automatically detect the running instance and establish a secure local connection (via a localhost port).
5.  **Exploration:** Open the Live State Telemetry panel. Use the Watchlist feature to pin your main character's health variable and your party's gold switch. See them update in real-time as you move in-game.

This initial setup takes less than five minutes. You are now ready to weave chaos into order.

## 🧑‍💻 Technical Architecture & Extensibility

The Chronicle Weaver adheres to a strict open architecture. All data is stored in a standard SQLite format, meaning you can export any telemetry report and analyze it with external tools. The suite provides a "Data Export" function that generates a clean, timestamped log of your playtest session in `.csv` or `.json` format for deeper statistical analysis.

**For Advanced Users:** The suite exposes a simple Command Line Interface (CLI) for automating batch profiler runs across multiple save files. This is perfect for nightly builds that need to verify that no variable achieved a "NaN" value during specific sequence triggers.

## ⚖️ License & Usage Agreement

This project is licensed under the **MIT License**, providing you with the freedom to use, modify, and distribute this toolkit in your personal and commercial projects, provided you retain the original copyright notice.

We believe in open tools for creative minds. Please see the [LICENSE](LICENSE) file for the full legal text.

## 🙏 Acknowledgments & Community

This project exists because of the vibrant, passionate community that has kept RPG Maker VX Ace alive for over a decade. We stand on the shoulders of scripters, eventers, and storytellers who pushed the engine to its limits. We are proud to contribute a tool that honors the complexity of their craft. We encourage you to share your "weaving" success stories, UI layout suggestions, and feature requests in our community hub.

---

## ⚠️ Disclaimer: A Note on Responsible Creation

The RPG Maker ACE Chronicle Weaver is a developmental aid. It is designed to provide you with deep insight into the **internal state** of your own game project during production. It does not facilitate the circumvention of copy protection, nor does it interfere with any Digital Rights Management (DRM) or external encryption schemes for commercial titles. The "Encryption Key Manager" is strictly a *recovery tool* for your own files lost due to hardware failure or accidental deletion—not a tool for bypassing others' security. We encourage creators to respect the intellectual property of others and use this suite solely to elevate the quality of their original stories. The responsibility for how you utilize this diagnostic power lies with you, the creator.