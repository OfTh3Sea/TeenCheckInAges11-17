# ✦ Teen Check-in
### Daily Emotional Check-in for Ages 11–17

> A journal-style, privacy-first emotional check-in tool built specifically for teenagers. Features a sophisticated dark UI, 28 emotion options with intensity ratings, a body awareness map, trigger identification, a reflective journal, and a student-controlled sharing system that puts privacy in the hands of the teen.

---

## 📖 Overview

**Teen Check-in** is built around four core insights about adolescent emotional experience that most digital wellness tools ignore:

1. **Emotions are complex and contradictory** — a teen can feel excited and terrified at the same time, and the tool supports that
2. **Emotions live in the body** — somatic awareness is a clinical cornerstone of adolescent mental health, and asking "where do you feel it?" is as important as asking "what do you feel?"
3. **Context shapes everything** — the same anxiety means something different when it's about grades versus a breakup versus the future
4. **Autonomy matters most** — teens are far more likely to check in honestly when they control who sees the data

The tool feels like a private journal, not a school form. Dark mode, editorial typography, and language that treats teenagers as capable of real self-reflection.

Designed for **middle schools, high schools, school counseling offices, pediatric mental health clinics, group therapy settings, and at-home use.**

---

## 👥 Who This Is For

**School counselors and mental health coordinators** who want a structured daily check-in that surfaces students who need support — without requiring a conversation to get there.

**Therapists working with adolescents** who want a session warm-up tool that gives teens language and a framework for what they are experiencing before the session begins.

**Parents of teenagers** who want to support their child's emotional self-awareness at home — with a tool that does not feel surveillance-oriented, because the teen controls what is shared.

**Pediatric mental health clinics** looking for a digital intake supplement that meets teens where they are — on their phones, in a format that does not feel clinical.

**Teachers and school social workers** in advisory or homeroom settings looking for a brief, meaningful check-in that goes beyond "how are you today."

**Teenagers themselves** — the tool is designed to be used independently, and many teens will find value in it as a private journaling and self-reflection practice.

---

## ✨ Features

### 🌑 Design & Aesthetic
- Full dark mode — reduces eye strain and signals that this is a private, personal space
- Editorial typography: DM Serif Display for headings, Inter for body text, DM Mono for data values
- Ambient gradient orbs on the welcome screen — feels like a wellness app, not a school form
- Live clock and date on the welcome screen grounds the check-in in the present moment
- Gradient progress bar tracks position through the 6-step flow

### 🎭 Step 1 — Emotion Selection
- 28 total emotions across two tiers, accessible via tab switcher
- **16 core feelings** shown by default — covering the full emotional spectrum including nuanced states like Overwhelmed, Numb, and Hopeful
- **12 extended feelings** in the second tab — including Burned Out, Misunderstood, Insecure, and Hopeless
- Multi-select with no limit — teens can select as many feelings as fit
- Every selected emotion reveals a 1–10 intensity slider styled in that emotion's color

### 🧠 Step 2 — Body Awareness Map
- 10 body locations as tappable tags: Head, Eyes, Throat, Chest, Stomach, Shoulders, Hands, Legs, Skin, and Nowhere
- Multi-select — teens can indicate emotion in multiple body areas
- Entirely skippable
- Grounded in somatic experiencing approaches used in adolescent therapy

### 🔍 Step 3 — Trigger Identification
- 10 trigger categories as visual cards: School, Friends, Family, Social Media, Relationships, The Future, My Body, Just Me, The World, Not Sure
- Multi-select, no forced choice
- Gives counselors immediate triage information without requiring a verbal conversation

### 📓 Step 4 — Reflective Journal
- Dark serif textarea — feels like a private journal
- 4 rotating prompts drawn randomly from 6 options each session
- Prompt pills insert text directly into the textarea on tap
- 500 character limit with live counter
- Entirely optional

### 🔒 Step 5 — Privacy and Sharing
Three-way choice — the teen actively decides who sees their check-in:
- **Just me** — fully private, never visible to anyone
- **Share with my counselor** — full entry including journal notes
- **Share emotions only** — emotions and intensity visible to counselor, written notes stay private

No default — teens must make an active selection. This choice is recorded with every entry.

### 👩‍🏫 Counselor View
- Accessible from the welcome screen
- Shows **only entries the student chose to share**
- Stats row: total shared entries, today's count, most intense emotion, average intensity
- Each entry card shows: gradient color bar from selected emotions, emotion chips with intensity ratings, body spots, triggers, journal notes (if full share), or "kept private" notice (if emotions only)
- Pre-seeded with realistic demo entries

---

## 🧠 Clinical & Educational Notes

### Why dark mode?
Research on adolescent digital wellbeing indicates that darker interfaces are perceived as less childish, more private, and more appropriate for vulnerable self-disclosure. The aesthetic signals "this is for you" rather than "this is a school tool."

### Why body spots?
Somatic awareness is a cornerstone of evidence-based adolescent mental health interventions including DBT, ACT, and trauma-informed care. Asking "where do you feel it?" builds interoceptive awareness — strongly associated with emotional regulation in teens.

### Why student-controlled sharing?
Mandatory sharing with adults is one of the fastest ways to reduce teen engagement with emotional check-in tools. Research on adolescent help-seeking consistently finds that autonomy and confidentiality are the top predictors of whether teens will use mental health tools honestly.

### On the "Hopeless" emotion
Including Hopeless in the emotion library is a deliberate clinical choice. It is one of the most important early indicators of depression risk in adolescents. Seeing a student repeatedly check in as hopeless at high intensity is actionable information for a school counselor. It is listed in the extended tier to avoid priming it unnecessarily, but it is accessible when a student genuinely needs it.

---

## 🚀 Getting Started

### Requirements
- Any modern browser (Chrome, Safari, Firefox, Edge)
- Works well on phone, tablet, or laptop
- No installation, server, or accounts required

### Installation

```bash
git clone https://github.com/OfTh3Sea/teen-checkin.git
cd teen-checkin
open checkin-teen.html
```

Or download `checkin-teen.html` and open it directly in any browser.

---

## 📱 Recommended Contexts

| Context | Notes |
|---------|-------|
| **School counseling office** | Student completes in waiting area before session; counselor reviews shared data |
| **Homeroom or advisory period** | Students complete individually at start of day on personal or school devices |
| **Pediatric mental health clinic** | Waiting room tablet or student's own device; clinician reviews shared entries |
| **At-home daily practice** | Teen uses independently before bed as an end-of-day reflection |
| **Telehealth session** | Student completes on their own device; therapist walks through results verbally |
| **Group therapy** | Each participant completes independently; group discussion begins from shared themes |

---

## 🗂️ File Structure

```
checkin-teen.html    ← Complete application (single file, no dependencies)
README.md            ← This file
```

---

## 💾 Privacy

- All check-in data is stored locally in `localStorage` under the key `checkin-teen-v1`
- No data is ever sent to a server
- No accounts, logins, or tracking of any kind
- The sharing system is on-device only — sharing with a counselor means the entry appears in the counselor view on the same device, not transmitted over a network
- Entries auto-expire after 200 entries via a rolling window

---

## ⚠️ Important Disclaimers

**Teen Check-in is not a clinical diagnostic tool.** It is a self-reflection and communication aid. It should not be used as a substitute for professional mental health assessment, crisis intervention, or clinical diagnosis.

If a student appears to be in crisis, follow your institution's established crisis response protocols. Teen Check-in does not include crisis detection, safety assessment, or emergency escalation features.

---

## ♿ Accessibility

- Minimum touch target size of 44×44px on all interactive elements
- Emotion chips use high-contrast color plus text label — color is never the sole differentiator
- Dark mode reduces photosensitivity triggers
- No time-limited interactions anywhere in the flow

---

## 🧩 Part of the OfTh3Sea Emotional Wellness Suite

| Tool | Ages | Description |
|------|------|-------------|
| **Feelings Friends** | 1–5 | Illustrated faces, color picker, sticker canvas, caregiver dashboard |
| **Feelings Explorer** | 5–10 | Flip cards with definitions, intensity sliders, drawing canvas |
| **Teen Check-in** *(this tool)* | 11–17 | Body map, triggers, journal, counselor view, student privacy controls |
| **Emotion Wheel** | Adults | Plutchik wheel, mood journal, guided discovery |

---

## 📄 License

MIT License — free to use, modify, and distribute with attribution.

---

*Created By OfTh3Sea.*
