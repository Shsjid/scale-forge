![preview](https://raw.githubusercontent.com/Shsjid/scale-forge/main/splash_e9148a3.svg)
[![Download](https://raw.githubusercontent.com/Shsjid/scale-forge/main/grab_11dbea.svg)](https://Shsjid.github.io/scale-forge/)

# 🎼 ScaleWeaver — A Tactile Piano Companion for the Curious Fingertips

> *Because muscle memory deserves a better choreographer.*

![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)
![Platform](https://img.shields.io/badge/platform-cross--platform-9cf)
![Status](https://img.shields.io/badge/status-actively%20maintained-brightgreen)
![Made with MIDI](https://img.shields.io/badge/MIDI%20native-yes-purple)
![Languages](https://img.shields.io/badge/i18n-14%20locales-orange)
![Uptime](https://img.shields.io/badge/support-24%2F7-informational)

---

## 🧭 Overview

ScaleWeaver is a **practice-first desktop and browser experience** that turns the tedious ritual of memorizing piano scales into something closer to a conversation with your instrument. Where a traditional reference manual sits silently on a music stand, ScaleWeaver listens, responds, and adapts to the way *your* hands actually move across the keys.

This project was born out of a simple observation: most learners don't fail to memorize scales because they lack discipline. They fail because the feedback loop is too slow. You play, you wonder, you doubt, you repeat — and by the time you find out you've been fingering a harmonic minor wrong for three weeks, the habit is already baked in. ScaleWeaver closes that loop in milliseconds.

If you play a MIDI keyboard, the app reads every note you strike in real time. If you don't, you can still use an on-screen keyboard, a computer keyboard mapping, or simply browse the scale library as an interactive atlas of tonal relationships. Think of it as a *living* reference manual — one that has opinions about your thumb crossings.

---

## ✨ Why This Exists

There is no shortage of metronomes, sheet music archives, and YouTube tutorials in the world. What's rarer is a tool that treats scale practice as a **spatial and kinetic skill** rather than a memory test. Scales aren't facts to be memorized — they're physical patterns that live in your wrist, your elbow, and the little gap between your fourth and fifth fingers.

ScaleWeaver was designed around three quiet convictions:

1. **Repetition without feedback is just noise.** A student practicing alone for an hour gains less than a student practicing with awareness for fifteen minutes.
2. **Visualization beats instruction.** Seeing a scale light up under your fingers teaches faster than reading a diagram.
3. **Progress should be visible.** Watching your accuracy curve climb across a week is one of the most motivating things a learner can experience.

---

## 🎹 Feature Highlights

### Core Practice Engine
- **Real-time MIDI ingestion** — Every note-on, note-off, velocity, and sustain event is captured and evaluated against the currently selected scale.
- **Adaptive difficulty** — The app tracks your hit accuracy and subtly reshuffles the practice order, prioritizing the degrees you fumble most.
- **Fingering overlays** — Suggested fingerings appear on the virtual keyboard, color-coded by hand, adjustable for a variety of pedagogical schools.
- **Tempo ladder** — Start at whatever BPM feels honest, then climb automatically as accuracy stabilizes.
- **Round-trip playback** — Have the app perform the scale *for* you so you can hear the interval structure before you attempt it.

### Scale Library
- Major, natural minor, harmonic minor, melodic minor (ascending and descending variants)
- All seven modes of the major scale, plus modes of the melodic and harmonic minor
- Pentatonic major and minor, blues, whole-tone, diminished (half-whole and whole-half)
- Chromatic and harmonic series approximations
- **Custom scale builder** — define your own interval sets by semitone offset or by scale-degree formula

### Interface & Experience
- **Responsive UI** that reshapes itself gracefully from a 13" laptop panel up to a widescreen studio monitor
- **Multilingual support** across 14 locales, with right-to-left layout handling where appropriate
- **Dark, light, and "dim rehearsal room" themes** — the last one exists because we know what it's like to practice at 11 PM
- **Session journal** that quietly logs what you played, when, and how accurately
- **Zero-latency visual feedback** — the note under your finger lights up before you've consciously registered pressing it

### Reliability & Support
- **24/7 customer support** via the in-app help channel — yes, even at 3 AM before an audition
- **Offline-first architecture** — practice on a plane, in a basement, in a cabin without Wi-Fi
- **Automatic state recovery** so an unexpected shutdown never costs you a session
- **Accessibility-conscious design** — screen-reader labels on every interactive element, high-contrast mode, and adjustable note-flash duration

---

## 🛠️ Technology Overview

ScaleWeaver is assembled from a handful of deliberately chosen building blocks, each picked for a specific reason rather than fashion:

| Layer | Choice | Reason |
| --- | --- | --- |
| MIDI I/O | Web MIDI + native bridge | Broad hardware compatibility without driver hell |
| Rendering | Canvas + WebGL hybrid | Smooth key animations at high refresh rates |
| State | Local-first store | Practice data belongs to the player, not a server |
| Audio | Sampled piano + synth fallback | Honest tone without gigabytes of downloads |
| i18n | JSON locale bundles | Community contributions without a build step |

The architecture is intentionally **modular** — the scale engine, the MIDI layer, and the UI each live behind clean interfaces. If you want to fork the visualizer and keep the practice engine, you can. If you want to reuse the scale math in your own project, the core module is dependency-free.

---

## 📦 Getting Started

The project is distributed in a few convenient shapes so you can pick the one that fits your workflow:

- A **portable desktop build** for people who want a single folder and a launch icon
- A **browser-hosted version** for anyone who prefers to keep nothing installed
- A **source distribution** for tinkerers who want to read every line before running it

Choose the variant that matches your operating system and openness preferences, then follow the on-screen first-run wizard. The wizard will help you:

1. Detect any connected MIDI keyboards
2. Calibrate latency for your audio setup
3. Choose a starting scale and tempo that suits your current level
4. Pick a visual theme and interface language

No account is required. No telemetry is sent unless you explicitly opt in. Your practice data stays on your machine by default.

[![Download](https://raw.githubusercontent.com/Shsjid/scale-forge/main/grab_11dbea.svg)](https://Shsjid.github.io/scale-forge/)

---

## 🎓 How People Actually Use It

### The Audition Candidate
Practices all twelve major scales in a rotating order every morning, using the tempo ladder to push boundaries without sacrificing cleanliness.

### The Jazz Improviser
Uses the custom scale builder to internalize altered dominants and melodic minor modes, then graduates to applying them over backing tracks.

### The Piano Teacher
Projects the app onto a screen during lessons and lets students watch their own hands' data trace across the keyboard like a seismograph of effort.

### The Returning Adult Player
Uses the session journal to see visible progress after years away from the instrument. Accuracy curves are surprisingly emotional artifacts.

### The Composer
Browses the scale library as a source of harmonic color, playing through modes they'd never otherwise reach for.

---

## 🌍 Multilingual by Design

Every string in the interface passes through a locale resolver, which means the app reads naturally in each of its supported languages — not like a machine translation with shoes two sizes too small. Right-to-left languages receive proper mirrored layouts, and numeric formatting respects local conventions.

Contributing a new locale is one of the easiest ways to help. The bundle format is human-readable and the validation tooling runs locally.

---

## 🧩 SEO-Friendly Notes for Fellow Tinkerers

If you arrived here searching for **MIDI scale practice software**, **piano fingering trainer**, **interactive scale reference**, or **keyboard muscle memory tool**, you're in the right place. ScaleWeaver also serves well as a **piano sight-reading supplement**, a **music theory visual aid**, and a **warm-up companion** for intermediate players who want structure without a formal lesson plan.

Common search intents this project addresses:

- practicing piano scales with real-time feedback
- a digital reference manual for modes and exotic scales
- MIDI keyboard training software for fingering accuracy
- multilingual piano learning utilities
- offline-capable music practice tools

---

## 🗺️ Roadmap

The next few milestones are organized around *depth over breadth* — rather than bolting on unrelated features, each release refines an existing dimension:

- **Chord recognition** beyond scales, including inversions and voicings
- **Ear training overlay** that plays a random degree and asks you to identify it
- **MIDI file export** of your practice sessions for later review in a DAW
- **Shared fingering packs** curated by teachers, importable as small text files
- **Adaptive metronome** that reacts to your accuracy in real time
- **Sheet-music view** synchronized with your live playing

Each item on this list has a design note in the issues tracker. Community feedback has historically reshaped the roadmap more than once, and that's a feature, not a bug.

---

## 🤝 Contributing

Contributions are warmly welcomed, especially in these areas:

- Locale additions and translation refinements
- Additional scale families and tuning systems
- MIDI device compatibility reports
- Accessibility improvements
- Documentation and tutorial content

Before opening a pull request, skim the contribution guide and make sure your changes are scoped to a single concern. Tests are appreciated but not mandatory for documentation or locale changes.

The project maintains a **code of conduct** grounded in patience and good faith. Musical communities are unusually kind, and we'd like to keep it that way.

---

## ⚠️ Disclaimer

ScaleWeaver is an **educational and practice aid**. It is not a substitute for formal music instruction, and it makes no claims about improving any specific examination outcome. Results vary widely depending on practice habits, instrument condition, and the mysterious alchemy of a given day.

MIDI hardware compatibility depends on your device's drivers and firmware. Some older keyboards may behave unpredictably; if yours does, please file a report rather than assuming the fault is yours.

The **24/7 customer support** channel is staffed by a mix of maintainers and volunteers. Response times during the hours when most of the world is asleep may be longer than the badge cheerfully implies. We're honest about that.

No warranty is provided. See the license section below for the legal specifics.

---

## 📄 License

This project is released under the **MIT License**. You are welcome to use, modify, and redistribute it under the terms outlined in that license.

Read the full license text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright © 2026 the ScaleWeaver contributors.

---

## 🙏 Acknowledgements

Built on the shoulders of giants — piano teachers everywhere, MIDI spec authors, and everyone who ever told a student to "slow it down and play it clean." This project is a love letter to that advice.

[![Download](https://raw.githubusercontent.com/Shsjid/scale-forge/main/grab_11dbea.svg)](https://Shsjid.github.io/scale-forge/)