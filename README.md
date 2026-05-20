# ✦ Check In
### Daily Emotional Check-in for Ages 11–17

> A journal-style, privacy-first emotional check-in tool built for teenagers. Features a sophisticated dark UI, 28 emotion options with intensity ratings, a body awareness map, trigger identification, a reflective journal, and a student-controlled sharing system for counselors.

---

## 📖 Overview

**Check In** is a single-file, browser-based emotional check-in tool designed specifically for adolescents aged 11–17. Where younger tools use bright colors and cartoon faces, Check In takes a different approach — dark mode, editorial typography, and language that treats teens as capable of real self-reflection.

The tool is built around four core insights about adolescent emotional experience:

1. **Emotions are complex and contradictory** — teens can feel excited *and* terrified at the same time, and the tool supports that
2. **Emotions live in the body** — somatic awareness is a clinical cornerstone of adolescent mental health work
3. **Context shapes everything** — the same feeling of anxiety means something different when it's about grades vs. a friendship
4. **Autonomy matters most** — teens are more likely to engage honestly when they control who sees their data

Designed for use in **middle schools, high schools, school counseling offices, pediatric mental health clinics, group therapy settings, and at-home wellness routines.**

---

## ✨ Features

### 🌑 Design & Aesthetic
- **Dark mode throughout** — reduces eye strain and feels more personal than clinical
- **Editorial typography** — DM Serif Display for headings (emotional, expressive), Inter for body text (clean, readable), DM Mono for data values (technical, precise)
- **Ambient gradient orbs** — subtle background lighting effect on the welcome screen
- **Live clock and date** — welcome screen shows the current day/time, grounding the check-in in the present moment
- **Gradient progress bar** — purple-to-lavender bar tracks position through the 6-step flow

### 🎭 Emotion Selection (Step 1)
- **28 total emotions** across two tiers — accessible via tab switcher
- **16 core feelings** shown by default, covering the full emotional spectrum
- **12 extended feelings** available via "More feelings" tab, including nuanced states like *burned out*, *misunderstood*, *insecure*, and *hopeless*
- **Multi-select** — no limit on the number of feelings selected simultaneously
- **Intensity sliders** — every selected emotion reveals a 1–10 slider styled in that emotion's color, with live numeric readout
- **Hover descriptions** — brief one-line descriptions appear on hover (desktop) to clarify emotion meanings

### 🧠 Body Awareness Map (Step 2)
- **10 body locations** presented as tappable tags — head, eyes, throat, chest, stomach, shoulders, hands, legs, skin, and "I don't feel it anywhere"
- Multi-select — teens can indicate emotion in multiple body areas simultaneously
- Entirely skippable with a single tap
- Grounded in somatic experiencing approaches used in adolescent therapy

### 🔍 Trigger Identification (Step 3)
- **10 trigger categories** as visual cards with icon, label, and descriptive subtitle
- Categories: School, Friends, Family, Social media, Relationships, The future, My body, Just me, The world, Not sure
- Multi-select, no forced choice
- Cards highlight in accent color when selected

### 📓 Reflective Journal (Step 4)
- **Dark serif textarea** — feels like a private journal, not a form field
- **4 rotating prompts** drawn randomly from 6 options each session
- Prompt pills insert text directly into the textarea on tap
- 500 character limit with live counter (DM Mono font)
- Entirely optional — skippable with a single tap

### 🔒 Privacy & Sharing (Step 5)
- **Three-way choice** — teens actively decide who sees their check-in:
  - 🔒 **Just me** — fully private, never visible to anyone
  - 🤝 **Share with my counselor** — full entry including journal notes
  - 📊 **Share emotions only** — emotions and intensity visible to counselor, written notes stay private
- This choice is recorded with every entry and surfaced in the counselor view
- No default — teens must make an active selection

### ✦ Done Screen
- Animated floating ✦ symbol
- Personalized message tied to their highest-intensity emotion (12 emotion-specific messages)
- Full summary card showing: emotions with intensity ratings, body locations, triggers, journal preview, and share status
- "New check-in" and "← Home" actions

### 👩‍🏫 Counselor View
- Accessible from the welcome screen footer link
- Shows **only entries the student chose to share**
- Stats row: total shared entries, today's count, most intense emotion, average intensity across all entries
- Each entry card shows: gradient color bar from all selected emotions, emotion chips with intensity ratings, body spots, triggers, journal notes (if full share), or "🔒 Note kept private" notice (if emotions-only share)
- Pre-seeded with 3 realistic demo entries covering anxiety, loneliness, and pre-game nerves
- Entries stored in `localStorage` and persist across sessions

---

## 🎭 Emotion Library

### Tier 1 — Core Feelings (16, shown by default)

| Emotion | Color | One-line Description |
|---------|-------|---------------------|
| Joy | `#f5c842` | Feeling genuinely happy |
| Excited | `#ff8c42` | Pumped up, can't wait |
| Proud | `#52d98a` | You did something good |
| Grateful | `#42c9b0` | Thankful for something |
| Calm | `#64b0f5` | Peaceful, settled |
| Hopeful | `#78d4a0` | Things might get better |
| Content | `#a0c878` | Not amazing, but okay |
| Loved | `#f57eb0` | Connected, cared for |
| Sad | `#6496d4` | Heavy, down, tearful |
| Anxious | `#d4a060` | Worried, what-if thinking |
| Angry | `#e85050` | Rage, injustice, heat |
| Frustrated | `#e07040` | Blocked, nothing working |
| Scared | `#b068d8` | Something feels threatening |
| Lonely | `#7896c0` | Disconnected, unseen |
| Overwhelmed | `#c060a8` | Too much at once |
| Numb | `#788090` | Flat, can't feel much |

### Tier 2 — Extended Feelings (12, via "More feelings" tab)

| Emotion | Color | One-line Description |
|---------|-------|---------------------|
| Embarrassed | `#e87890` | Awkward, want to disappear |
| Jealous | `#70b890` | Wishing you had what they have |
| Guilty | `#9878c0` | Did something that feels wrong |
| Confused | `#c0a850` | Nothing makes sense right now |
| Disappointed | `#8080b8` | Expected more, got less |
| Restless | `#d4784a` | Can't settle, need to move |
| Insecure | `#b09080` | Doubting yourself |
| Hopeless | `#607090` | Can't see a way forward |
| Burned out | `#a07860` | Completely empty, done |
| Supported | `#50a8d8` | Someone has your back |
| Misunderstood | `#9898b8` | Nobody gets it |
| Determined | `#60c870` | Focused, won't give up |

---

## 🔍 Trigger Categories

| Icon | Category | Covers |
|------|----------|--------|
| 📚 | School | Classes, grades, homework, tests |
| 👥 | Friends | Friendships, social stuff, drama |
| 🏠 | Family | Home life, parents, siblings |
| 📱 | Social media | Online stuff, comparison, FOMO |
| 💌 | Relationships | Crush, dating, breakup |
| 🌫️ | The future | What happens next, uncertainty |
| 🪞 | My body | How I look, health, changes |
| 💭 | Just me | My thoughts, feelings about myself |
| 🌎 | The world | News, climate, big things |
| ❓ | Not sure | I can't quite pinpoint it |

---

## 📓 Journal Prompts

Each session randomly displays 4 of these 6 prompts:

- *"What happened today that stands out?"*
- *"What do I wish someone understood about how I'm feeling?"*
- *"If this feeling had a color or shape, what would it be?"*
- *"What do I need right now?"*
- *"What's one thing that would make tomorrow feel better?"*
- *"Is there something I've been avoiding thinking about?"*

---

## 🚀 Getting Started

### Requirements
- Any modern browser (Chrome, Safari, Firefox, Edge)
- No server, build tools, or dependencies required
- Works offline after initial load (Google Fonts requires a connection on first visit)

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/checkin-teen.git

# Navigate into the project
cd checkin-teen

# Open in your browser
open checkin-teen.html
```

Or simply **download `checkin-teen.html`** and open it in any browser. No setup required.

---

## 📱 Recommended Usage

| Setting | Device | Notes |
|---------|--------|-------|
| School counselor's office | Laptop or tablet | Counselor and student use same device; student completes check-in privately |
| Homeroom / advisory period | School Chromebook or tablet | Students complete individually at start of day |
| Group therapy | Shared tablet or individual devices | Each student's choices stay on their device |
| Pediatric mental health clinic | Waiting room tablet | Dark mode reduces anxiety in clinical environments |
| At-home daily routine | Phone or laptop | Works well before bed as an end-of-day reflection |
| Telehealth session | Student's own device | Therapist walks through prompts verbally; student controls sharing |

**Note for counselors:** The counselor view is password-free by design — requiring a password would complicate tablet sharing in school settings. If you need access control, host the file on a device the student doesn't have access to outside of sessions, or work with your IT team on device-level access controls.

---

## 🗂️ File Structure

```
checkin-teen.html    ← Entire application (single file, zero dependencies)
README.md            ← This file
```

This is a **single-file application** by design. All HTML, CSS, JavaScript, emotion data, and logic are bundled into one portable file. It can be emailed, shared via USB, hosted on any static server, or added to a school's intranet without any configuration.

---

## 🖼️ App Flow

```
┌──────────────────────────────────────────────────────────────┐
│                      WELCOME SCREEN                           │
│                  [ambient gradient orbs]                      │
│            Monday, June 9, 2025 · 8:47 AM                    │
│                                                               │
│               How are you                                     │
│               really doing?                                   │
│                                                               │
│     · 2–3 minutes · No wrong answers · Your choice to share  │
│                                                               │
│                  [ Start check-in ]                           │
│             Counselor / caregiver view →                      │
└──────────────────────┬───────────────────────────────────────┘
                       │
          ─────────────▼─────────────
          Step 1: What are you feeling?
          ─────────────────────────────
          [ Core feelings ] [ More feelings ]   tabs
          
          ● Joy  ● Excited  ● Proud  ● Calm     chips
          ● Sad  ● Anxious  ● Angry  ● Lonely   (multi-select)
          ...
          
          Selected emotions show intensity sliders:
          Anxious  ━━━━━━━━●━━  8/10
          Lonely   ━━━━━━●━━━━  6/10
          
                       │
          ─────────────▼─────────────
          Step 2: Where do you feel it?
          ──────────────────────────────
          🧠 Head   💗 Chest   🌀 Stomach   ✋ Hands
          🫁 Throat  🏋️ Shoulders  🦵 Legs    🌡️ Skin
          👁️ Eyes   😶 I don't feel it anywhere
          
                       │
          ─────────────▼─────────────
          Step 3: What's it connected to?
          ─────────────────────────────────
          ┌──────────┐  ┌──────────┐  ┌──────────┐
          │ 📚       │  │ 👥       │  │ 📱       │
          │ School   │  │ Friends  │  │ Social   │
          │ Classes, │  │ Social   │  │ media    │
          │ grades…  │  │ drama…   │  │ FOMO…    │
          └──────────┘  └──────────┘  └──────────┘
          
                       │
          ─────────────▼─────────────
          Step 4: Anything else?
          ─────────────────────────────
          [ What happened today? ]  [ What do I need? ]   prompts
          
          ╔════════════════════════════════╗
          ║  I have three tests next week  ║
          ║  and I can't stop thinking     ║  journal textarea
          ║  about all of them at once…   ║
          ╚════════════════════════════════╝
          247 / 500
          
                       │
          ─────────────▼─────────────
          Step 5: Who sees this?
          ─────────────────────────────
          🔒 Just me
          🤝 Share with my counselor
          📊 Share emotions only
          
          [ Save my check-in ]
          
                       │
          ─────────────▼─────────────
          ✦  Check-in complete.
          ─────────────────────────────
          Summary: emotions · body · triggers · note · share status
```

---

## 💾 Data & Privacy

### What is stored
- All check-in data is stored in the browser's `localStorage` under the key `checkin-teen-v1`
- Each entry contains: timestamp, selected emotions with intensities, body spots, triggers, journal text, and share choice

### What is NOT stored or transmitted
- **No data ever leaves the device**
- No analytics, telemetry, or usage tracking of any kind
- No accounts, logins, or user identifiers
- No cookies

### The sharing system
The sharing system is **on-device only** — "sharing with a counselor" means the entry appears in the counselor view on the same device. No data is sent to the counselor over a network. For true multi-device sharing, you would need to implement a backend (see [Contributing](#-contributing)).

### Student data rights
- Students can see all their own entries by opening the counselor view
- No mechanism exists to delete individual entries from the UI (entries auto-expire after 200 entries via a rolling window — oldest entries are removed when the limit is reached)
- Clearing browser/site data removes all entries completely

> ⚠️ **For schools and clinics:** Because data is stored in `localStorage`, it is tied to the specific browser on the specific device. If a student completes a check-in on the school's shared iPad and then clears the browser, the data is gone. For persistent, multi-session tracking consider implementing a simple backend or exporting entries periodically.

---

## 🧠 Clinical & Educational Notes

### Why dark mode?
Research on adolescent digital wellbeing suggests that darker interfaces are perceived as less childish, more private, and more appropriate for vulnerable self-disclosure. The aesthetic signals "this is serious and for you" rather than "this is a school tool being done to you."

### Why body spots?
Somatic awareness is a cornerstone of evidence-based adolescent mental health interventions including **DBT** (Dialectical Behavior Therapy), **ACT** (Acceptance and Commitment Therapy), and **trauma-informed care**. Asking "where do you feel it?" builds interoceptive awareness — a skill strongly associated with emotional regulation in teens.

### Why trigger categories?
Adolescent distress is almost always contextual. The same level of anxiety means something clinically different when it's school-related vs. body-image-related vs. family-related. Trigger data gives counselors immediate triage information without a conversation.

### Why student-controlled sharing?
Mandatory sharing with adults is one of the fastest ways to reduce teen engagement with emotional check-in tools. Research on adolescent help-seeking consistently finds that **autonomy and confidentiality** are the top predictors of whether teens will use mental health tools honestly. By letting students choose, you get more truthful data, not less.

### On the "Hopeless" emotion
Including *hopeless* in the emotion library is a deliberate clinical choice. It is one of the most important early indicators of depression risk in adolescents. Seeing a student repeatedly check in as "hopeless" at high intensity is actionable information for a school counselor. The emotion is listed in Tier 2 to avoid priming it unnecessarily, but it is accessible when a student genuinely needs it.

---

## 🔧 Customization

### Adding or editing emotions

```javascript
// In the EMOTIONS array:
{
  id: 'your-emotion',       // unique snake-case ID
  label: 'Your Emotion',    // display name (sentence case)
  color: '#hexcolor',       // used for chip, slider, and counselor card
  tier: 1,                  // 1 = core (shown by default), 2 = extended tab
  desc: 'Brief description' // shown on hover (desktop) — one short phrase
}
```

### Adding journal prompts

```javascript
const JOURNAL_PROMPTS = [
  'What happened today that stands out?',
  'Your new prompt here — keep it open-ended',
  // Add as many as you like — 4 are shown per session, drawn randomly
];
```

### Adding trigger categories

```javascript
const TRIGGERS = [
  {
    id: 'your-trigger',
    icon: '🎯',              // emoji icon
    label: 'Category Name',  // short label on card
    sub: 'Longer description of what this covers'
  },
  // ...
];
```

### Adding body spots

```javascript
const BODY_SPOTS = [
  {
    id: 'jaw',
    icon: '😬',
    label: 'Jaw / clenched'
  },
  // ...
];
```

### Changing the storage key

If you're deploying multiple versions of this tool (e.g., different schools), change the storage key to prevent data collisions:

```javascript
const STORE = 'checkin-teen-schoolname-v1'; // customize per deployment
```

---

## ♿ Accessibility

- All interactive elements are keyboard-accessible where applicable
- Emotion chips use high-contrast color + text label (color is never the sole differentiator)
- Minimum touch target size: 44×44px on all interactive elements
- Body spot and trigger cards are large enough for motor-impaired users
- `user-scalable=no` is set to prevent accidental zoom — remove this from the `<meta>` tag if accessibility zoom is required
- Dark mode reduces photosensitivity triggers
- No time-limited interactions anywhere in the flow
- Live clock updates every 30 seconds (not a focus trap)

---

## 🧩 Part of a Larger Suite

Check In is part of a multi-tool emotional wellness ecosystem:

| Tool | Ages | Key Differentiator |
|------|------|--------------------|
| **Feelings Friends** | 1–5 | No reading required; illustrated faces; sticker canvas; caregiver dashboard |
| **Feelings Explorer** | 5–10 | Flip cards with definitions; intensity sliders; finger drawing canvas |
| **Check In** *(this tool)* | 11–17 | Dark mode; body map; triggers; journal; student-controlled privacy |
| **Mindscape** | Adults | Full Plutchik emotion wheel; CBT-inspired tools; mood journal |

Each tool is a standalone HTML file. They can be deployed independently or linked from a shared landing page.

---

## 🤝 Contributing

Contributions are welcome, especially from:
- School counselors and psychologists with clinical feedback
- Educators with classroom implementation experience
- Developers with accessibility expertise
- Translators for multilingual support

### Feature ideas

- [ ] Multi-language support (Spanish, Mandarin, Arabic, French, etc.)
- [ ] Backend integration for true multi-device counselor sync
- [ ] Weekly/monthly trend visualization for the counselor view
- [ ] Export check-in history as PDF or CSV
- [ ] Flagging system — counselors can mark entries that need follow-up
- [ ] Anonymous mode — counselor sees data with no identifier attached
- [ ] Offline PWA support via service worker
- [ ] Screen reader / keyboard navigation improvements
- [ ] Customizable emotion sets per school or clinic

### How to contribute

```bash
# Fork the repository on GitHub, then:
git clone https://github.com/your-username/checkin-teen.git
git checkout -b feature/your-feature-name

# Make your changes to checkin-teen.html
# Test in Chrome, Safari (iOS), and Firefox before submitting

git commit -m "Add: clear description of your change"
git push origin feature/your-feature-name
# Open a Pull Request — describe your change and why it matters
```

Please test on a phone-sized screen (375px wide) — many students will use this on a personal phone.

---

## ⚠️ Important Disclaimers

**Check In is not a clinical diagnostic tool.** It is a self-reflection and communication aid. It should not be used as a substitute for professional mental health assessment, crisis intervention, or clinical diagnosis.

**If a student appears to be in crisis**, follow your institution's established crisis response protocols. Check In does not include crisis detection, safety assessment, or emergency escalation features.

**The "Hopeless" and "Numb" emotions** in the extended tier are included to support honest self-expression. Counselors should treat repeated high-intensity check-ins with these emotions as a prompt for a direct conversation — not an automated alert.
```

---

## 🙏 Acknowledgments

- Emotion vocabulary informed by research on **emotional granularity** in adolescence (Lisa Feldman Barrett)
- Somatic awareness approach draws on **DBT** and **somatic experiencing** frameworks for adolescent mental health
- Trigger taxonomy developed in consultation with school counseling best practices
- Student-controlled privacy model inspired by research on **adolescent help-seeking behavior** and barriers to mental health service use
- Dark mode and journal aesthetic informed by qualitative research on teen digital wellness tool adoption

---

*Built for teenagers who are trying to figure out what they feel — and the adults who want to help.*
