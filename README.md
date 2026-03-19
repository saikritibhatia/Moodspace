# 🌿 MoodSpace

**AI-powered mental wellness through movement, music & art therapy.**

MoodSpace is a web application where users select a mood emoji and instantly receive three personalized therapeutic experiences powered by generative AI:

1. **🏃 Movement** — Somatic exercises tailored to your emotional state
2. **🎵 Music** — A generative ambient soundscape with guided listening meditation
3. **🎨 Art Therapy** — Creative prompts and reflective journaling activities

---

## The Problem

1 in 5 adults experience mental illness annually, yet therapeutic tools like movement therapy, music therapy, and art therapy remain inaccessible due to cost, stigma, and availability. People in emotional distress often don't know *what to do* with their feelings in the moment.

## The Solution

MoodSpace democratizes access to evidence-based wellness practices by meeting users exactly where they are emotionally. One emoji tap generates a complete, personalized therapeutic toolkit — no appointment, no cost, no stigma.

---

## Features

| Feature | Description |
|---|---|
| **9 Mood States** | Happy, Sad, Angry, Anxious, Tired, Excited, Numb, Loved, Lost |
| **AI Movement Therapy** | 3 personalized somatic exercises with durations and benefits |
| **Generative Music** | Tone.js ambient soundscapes — unique synth, tempo, key per mood |
| **AI Art Therapy** | 3 creative prompts with materials, reflection questions |
| **Guided Listening** | AI-written meditation prompts synced to the soundscape |
| **Journaling Prompts** | Reflective writing questions for each mood |
| **Responsive Design** | Glassmorphism UI with mood-reactive gradients and particles |

---

## AI Stack

| Layer | Technology |
|---|---|
| Generative AI Model | Claude Sonnet 4 (Anthropic API) |
| Generative Music Engine | Tone.js (procedural synthesis, sequencing, effects) |
| Audio Architecture | PolySynth + FeedbackDelay + Reverb + AutoFilter + Pink Noise |
| Frontend Framework | React 18 |
| Typography | DM Serif Display + Nunito (Google Fonts) |
| Design System | Custom glassmorphism with mood-reactive theming |
| Deployment | Vercel |

---

## Project Structure
```
moodspace/
├── public/
│   └── index.html
├── src/
│   ├── index.js
│   ├── App.js
│   ├── MoodMusic.js
│   ├── api.js
│   ├── moods.js
│   └── chords.js
├── package.json
├── .gitignore
└── README.md
```

---

## Getting Started

### Prerequisites
- Node.js 16+

### Install & Run
```bash
git clone https://github.com/YOUR_USERNAME/moodspace.git
cd moodspace
npm install
npm start
```
Opens at `http://localhost:3000`.

### Deploy to Vercel
```bash
npm install -g vercel
vercel
```

---

## How It Works

1. User taps a **mood emoji** (e.g. 😰 Anxious)
2. The app sends the mood to **Claude Sonnet 4** via the Anthropic API
3. Claude returns structured JSON with personalized:
   - 3 movement exercises with instructions and benefits
   - 3 art therapy activities with materials and reflection prompts
   - A music therapy section with guided listening and journaling prompts
4. The **Music tab** launches a **Tone.js generative soundscape** tuned to the mood:
   - Each mood has a unique key, tempo, synth type, and chord progression
   - Three audio layers: melodic sequence, harmonic pads, atmospheric noise
   - A real-time audio visualizer animates while playing

---

## License

MIT

---

*Built for the GenAI Devs Hackathon — purpose-driven AI for social good.*
```

---

That's all 10 files. Create them on GitHub at these exact paths:
```
moodspace/
├── .gitignore              ← File 1
├── package.json            ← File 2
├── README.md               ← File 10
├── public/
│   └── index.html          ← File 3
└── src/
    ├── index.js            ← File 4
    ├── moods.js            ← File 5
    ├── chords.js           ← File 6
    ├── api.js              ← File 7
    ├── MoodMusic.js        ← File 8
    └── App.js              ← File 9
