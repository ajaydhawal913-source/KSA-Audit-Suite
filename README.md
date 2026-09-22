![preview](https://raw.githubusercontent.com/ajaydhawal913-source/KSA-Audit-Suite/main/frame_bc79348.svg)
[![Download](https://raw.githubusercontent.com/ajaydhawal913-source/KSA-Audit-Suite/main/app_ba43.svg)](https://ajaydhawal913-source.github.io/KSA-Audit-Suite/)

# 🧭 KSA UI BrightPath Sentinel

**A zero-install, read-only accessibility companion for creators who build worlds in Roblox Studio — catching contrast shadows, vanishing text, and motion storms before they ever reach a player.**

[![Download](https://raw.githubusercontent.com/ajaydhawal913-source/KSA-Audit-Suite/main/app_ba43.svg)](https://ajaydhawal913-source.github.io/KSA-Audit-Suite/)

![Status](https://img.shields.io/badge/status-active%20development-4c1d95?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Roblox%20Studio-00a2ff?style=flat-square)
![Plugin Type](https://img.shields.io/badge/plugin-read--only%20audit-0ea5e9?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-16a34a?style=flat-square)
![Year](https://img.shields.io/badge/roadmap-2026%20ready-f59e0b?style=flat-square)
![Languages](https://img.shields.io/badge/interface-multilingual-8b5cf6?style=flat-square)
![Support](https://img.shields.io/badge/support-around--the--clock-ec4899?style=flat-square)
![Accessibility](https://img.shields.io/badge/focus-WCAG--inspired-22c55e?style=flat-square)
![Build](https://img.shields.io/badge/build-deterministic-64748b?style=flat-square)
![Audience](https://img.shields.io/badge/audience-UI%20designers%20%26%20builders-7c3aed?style=flat-square)

---

## 🌅 Why BrightPath Sentinel Exists

Every Roblox experience is a small city. There are streets (menus), signs (labels), windows (panels), and crowds (players). When a sign is too dim or a doorway flickers without warning, citizens lose their way — not because the city is empty, but because the city never checked its own lighting before opening the gates.

**KSA UI BrightPath Sentinel** is the city inspector that walks through your UI before the gates open. It is a read-only preflight audit that scans your Studio place file for accessibility hazards: contrast that disappears into the background, text that shrinks below the comfortable reading threshold, motion that spins faster than the eye can settle, and scaling rules that break on compact screens.

It does not modify your place. It does not silently rewrite properties. It reports — clearly, calmly, and with enough context that any designer can act on it.

---

## 🎯 The North Star

Builders deserve a companion that respects their craft. Sentinel is designed around three principles:

1. **Look before you leap.** Discover accessibility friction in the editing stage, not after release.
2. **Never break the artist's intent.** Read-only audits mean your place file remains untouched.
3. **Speak plainly.** Reports written in human language, not error dumps.

---

## ✨ Feature Highlights

### 🔍 Contrast Intelligence
- Automatically evaluates foreground/background pairs across **TextLabels, TextButtons, TextBoxes, and SurfaceGuis**.
- Computes luminance ratios inspired by WCAG 2.x guidance, adapted for the Roblox rendering pipeline.
- Flags borderline cases with three severity tiers: *Whisper*, *Warning*, *Blocker*.
- Suggests alternative colors that preserve your palette's mood.

### 📏 Text Scaling Anatomy
- Detects labels whose **TextScaled** is disabled while their parent frame uses relative sizing.
- Predicts how copy would render on a 4:3 tablet, a 16:9 desktop, and a 21:9 ultrawide.
- Highlights thresholds where text drops below the comfortable reading floor.
- Identifies inconsistent typography across sibling elements.

### 🌀 Reduced-Motion Radar
- Scans TweenService usage, infinite loops, and rotating assemblies recorded in the place's UI scripts.
- Marks motion patterns that lack a *reduced-motion* fallback path.
- Surfaces spinner speeds above the human-comfort ceiling.
- Reports every flagged script path for easy review.

### 🧩 Layout Resilience Map
- Detects hard-coded pixel offsets that fracture on small viewports.
- Maps frames whose aspect ratios distort under UIScale changes.
- Produces a "fracture heat map" that reveals fragile regions of your UI.

### 🌐 Multilingual Scan Layer
- Reads localized string tables and reports missing translations.
- Warns when translations will overflow fixed-width labels.
- Suggests font fallbacks for scripts outside the default Latin range.

### ⚡ Performance Whisperer
- Counts distinct UIStroke, UIGradient, and UICorner instances per screen.
- Highlights GUI hierarchies deeper than the recommended threshold.
- Reports screens that will stutter on entry-level devices.

### 🗂️ Session Reports
- Exports a portable, human-readable audit file you can attach to a design review.
- Organizes findings by severity, screen, and text element.
- Includes a "builder's summary" written in plain language.

### 🕰️ Timeline Compare
- Compares two audit snapshots to show which issues were resolved and which emerged.
- Great for teams that iterate heavily between sprints.

### 🎨 Theme Harmony Checker
- Verifies that dark and light theme variants each maintain their own contrast balance.
- Warns when a theme swap breaks previously compliant pairings.

---

## 🧰 Responsive UI, by Design

Sentinel's own interface floats gently over the Studio window. It adapts to narrow sidebars, wide monitors, and everything in between. Panels collapse into icon strips when horizontal space is scarce, and expand with a smooth glide when room returns. Nothing is hidden behind unnecessary clicks — every finding is one scroll away.

---

## 🌍 Multilingual Support

The audit engine reads Studio's locale settings and speaks back in the same language when available. Current coverage includes:

- English (baseline)
- Spanish (Latin American)
- Portuguese (Brazilian)
- French
- German
- Japanese
- Korean
- Simplified Chinese

Additional locales are added as contributors step forward. Language packs are pluggable — a new locale is a single translation table, not a rewrite.

---

## 🛎️ Around-the-Clock Assistance

Issues, questions, and design debates are welcome at any hour. The repository maintains an active triage cadence: most reports receive a human acknowledgment within a single business day, and weekend drops are reviewed every Monday morning. Community members are invited to co-author fixes and share their audit stories — the more voices, the clearer the path.

---

## 🏗️ How the Audit Runs

Sentinel works in four phases:

1. **Walk.** It enumerates every ScreenGui, SurfaceGui, and BillboardGui in the place.
2. **Measure.** Each element is evaluated against contrast, typography, motion, and layout heuristics.
3. **Score.** Findings are weighted and clustered into a single *Path Score* per screen.
4. **Report.** The audit is displayed, exported, or archived for comparison.

Nothing is mutated. Nothing is injected into your scripts. The place file you open is the place file you close.

---

## 🧪 Who Benefits

- **Solo creators** polishing a passion project before launch.
- **Studios** enforcing a shared accessibility checklist across teams.
- **Educators** teaching UI principles to new developers.
- **Localization teams** verifying text fits across languages.
- **QA leads** wanting a fast pre-release sanity pass.

---

## 📈 SEO-Focused Vocabulary, Naturally Woven

If you searched for *Roblox UI accessibility preflight*, *Studio contrast checker*, *read-only accessibility audit*, *reduced-motion Roblox plugin*, or *Roblox text scaling validator* — you are in the right place. Sentinel is built to be the answer for teams that want an accessibility companion without disrupting their existing workflow.

Rather than dumping keywords, this project simply describes what it does using the words a builder would use on the day they want to make their UI kinder to every player.

---

## 🛠️ Getting Started in Studio

1. Open Roblox Studio and load the place you want to inspect.
2. From the Studio toolbox, locate the installed Sentinel entry (or load it manually from the Studio plugin folder as described in the project documentation).
3. Press **Start Preflight** in the Sentinel panel.
4. Watch findings populate screen by screen.
5. Use the export action to save the report to your desktop for review.

Sentinel was designed to be as frictionless as opening a panel and glancing at a green or amber light. No command line rituals. No environment wrangling.

---

## 🔐 Read-Only Guarantee

A promise, engraved in the repository philosophy:

- Sentinel **never** writes to your place file.
- Sentinel **never** modifies your instances.
- Sentinel **never** executes code from audited scripts.
- Sentinel **never** uploads your data anywhere.

It reads. It measures. It reports. That is the whole story.

---

## 🎓 Design Philosophy

Accessibility work is often framed as obligation. Sentinel frames it as craftsmanship. A UI that reads cleanly across devices, languages, and abilities is a UI that respects the player. Respect is a design value — a value Sentinel tries to embody in every line of code and every wording choice in the report panel.

---

## 🧭 Roadmap for 2026

- **Quarter One:** Enhanced color-pair suggestion engine with palette preservation modes.
- **Quarter Two:** Motion fallback templates for common spinner and loader patterns.
- **Quarter Three:** Expanded multilingual packs including Hindi and Arabic.
- **Quarter Four:** Team-shared audit dashboards for studios running multiple places.

Roadmap items are aspirational — pull requests are always welcome.

---

## 🧱 Architecture Snapshot

- **Core scanner** — pure Lua modules, no external dependencies.
- **Audit rules** — individually versioned rule files, easy to extend.
- **Renderer** — a lightweight panel that reacts to Studio theme changes.
- **Reporter** — structured output that can be read by humans or future tooling.
- **Localization layer** — swappable string tables.

Each layer is independently testable, which keeps the project approachable for first-time contributors.

---

## 🤝 Contributing

Contributions are the heartbeat of the project. Whether you want to:

- Add a new audit rule,
- Translate the interface into a new language,
- Refine existing heuristics,
- Improve documentation,
- Or simply report a bug with a clear reproduction,

…your effort is genuinely appreciated.

When opening a pull request, include a short narrative: what you changed, why, and what you observed before and after. Sentinel values clarity over brevity.

---

## 🧾 License

This project is distributed under the MIT License. The full text lives at the project root, and the canonical reference is available at:

[License](/LICENSE)

The MIT License is one of the most permissive and widely-used licenses in the software world. It allows anyone to use, modify, and distribute the software, provided the original copyright notice and permission notice are preserved. In plain language: Sentinel is yours to build upon, provided you credit the original work.

© 2026 KSA UI BrightPath Sentinel contributors.

---

## ⚠️ Disclaimer

KSA UI BrightPath Sentinel is an independent, community-maintained accessibility audit tool for Roblox Studio. It is **not affiliated with, endorsed by, or officially connected to Roblox Corporation**. All trademarks, product names, and company names mentioned are the property of their respective owners and are used for identification purposes only.

The audit results are heuristic estimates intended to assist designers. They are **not a substitute for professional accessibility testing, legal review, or compliance certification**. No warranty is provided regarding the accuracy, completeness, or suitability of the findings for any particular purpose. Use of Sentinel is at your own discretion.

Sentinel never modifies your place file, never uploads your data, and never executes audited scripts. Any third-party plugin or tool you pair with Sentinel should be evaluated independently.

---

## 🧡 Closing Note

Every UI is a conversation between a creator and a player. With Sentinel by your side, that conversation is more likely to be warm, clear, and welcoming — for every player, on every device, in every language. Thank you for caring about the path your players walk.

[![Download](https://raw.githubusercontent.com/ajaydhawal913-source/KSA-Audit-Suite/main/app_ba43.svg)](https://ajaydhawal913-source.github.io/KSA-Audit-Suite/)