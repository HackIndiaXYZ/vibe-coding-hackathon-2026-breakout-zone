<div align="center">

<img src="https://github.com/iammissmiller/BreatheSafe/blob/main/src/banner.png?raw=true" alt="BreatheSafe Banner" width="100%"/>

<br/>
<br/>

[![Live Demo](https://img.shields.io/badge/Live%20Demo-breathe--safe--jet.vercel.app-1D9E75?style=for-the-badge&logo=vercel&logoColor=white)](https://breathe-safe-jet.vercel.app)
[![License: MIT](https://img.shields.io/badge/License-MIT-0F6E56?style=for-the-badge)](LICENSE)
[![Open Source](https://img.shields.io/badge/Open%20Source-%E2%9D%A4-5DCAA5?style=for-the-badge)](https://github.com/iammissmiller/BreatheSafe)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-9FE1CB?style=for-the-badge)](https://github.com/iammissmiller/BreatheSafe/pulls)

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://github.com/iammissmiller/BreatheSafe)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://github.com/iammissmiller/BreatheSafe)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://github.com/iammissmiller/BreatheSafe)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)](https://firebase.google.com)
[![Vercel](https://img.shields.io/badge/Deployed%20on-Vercel-000?style=flat-square&logo=vercel)](https://vercel.com)
[![Groq](https://img.shields.io/badge/AI-Groq-FF4B00?style=flat-square)](https://groq.com)

<br/>

> *Every breath should feel safe.*
>
> **BreatheSafe** monitors your air, navigates you away from pollution, guides you through breathing emergencies,  
> and gives you personalized respiratory intelligence — in real time, wherever you are.

<br/>

</div>

---

## 📽️ Demo

<div align="center">

<!-- 🎬 VIDEO PLACEHOLDER — Replace this section with your demo embed once recorded -->

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│            🎬  Demo Video Coming Soon                       │
│                                                             │
│   Record a walkthrough covering:                            │
│   • Onboarding quiz & profile setup                         │
│   • Live AQI dashboard with your location                   │
│   • SafeRoute — picking the cleanest path                   │
│   • HelpZone — triggering an AI emergency protocol          │
│   • Symptom Logger & Analytics dashboard                    │
│                                                             │
│   Recommended: Loom or OBS · 2–4 mins · 1080p              │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**👉 [Try it live instead →](https://breathe-safe-jet.vercel.app)**

</div>

---

## 🌍 Why BreatheSafe Exists

Over **300 million people** live with asthma. Hundreds of millions more are silently affected by urban air pollution every single day — stepping outside into air that triggers symptoms they can't measure, taking routes drenched in PM2.5, and facing breathing emergencies with no real-time guidance.

The tools that exist are either:
- **Too clinical** — hospital apps and spirometers aren't built for daily life
- **Too generic** — weather apps give AQI numbers with no context on what to *do*
- **Too reactive** — they tell you what happened, not what to do *right now*

**BreatheSafe fills that gap.**

It is the first app that combines live environmental data, AI-powered emergency action, personalized health profiling, clean route navigation, and emotional UX — all in one place, accessible to anyone with a browser.

> *"No one should face a breathing crisis alone, uninformed, or unprepared."*
> — Praptee Miller, Creator

This project supports **UN Sustainable Development Goals:**

| Goal | Alignment |
|------|-----------|
| 🏥 **SDG 3** — Good Health & Well-Being | Emergency breathing support, symptom tracking, health analytics |
| 🏙️ **SDG 11** — Sustainable Cities | Route optimization for clean air exposure in urban environments |
| 🌱 **SDG 13** — Climate Action | Real-time air quality awareness that drives environmental consciousness |

---

## ✨ Core Features

### 🆘 HelpZone — AI Emergency Protocol
> *Like having a paramedic in your pocket.*

Select your symptoms — asthma attack, hyperventilation, dust exposure, anxiety-triggered breathlessness — and HelpZone generates a **real, timed, step-by-step AI action plan**: exact body positions, breathing counts, medication reminders, countdown timers. Every episode is saved to your Analytics for pattern recognition. This is not generic advice. It is personalized to your health profile, severity level, and current environment.

---

### 🌫️ Air Quality Dashboard
> *Know what you're breathing before you step outside.*

Live AQI, PM2.5, humidity, wind speed, and UV index — pulled from your **exact GPS coordinates** via the OpenWeather API. Color-coded severity indicators, personalized health alerts based on your respiratory profile, and historical data to see how your local air quality trends over time.

---

### 🗺️ SafeRoute — Pollution-Aware Navigation
> *Don't just get there. Get there breathing.*

Powered by **OSRM routing + Leaflet.js**, SafeRoute calculates real road routes and overlays live AQI data color-coded along each path. Compare multiple routes side-by-side — not just by time or distance, but by **air quality exposure**. An AI health summary tells you what to expect on your journey and how to prepare.

---

### 🤖 AI Assistant
> *Your personalized respiratory advisor.*

Groq AI (llama-3.1-8b-instant) generates a fully personalized action plan based on your health profile, current AQI, logged symptoms, and environmental context. Updated in real time. Not a chatbot — a structured, timed guidance system built for breathing recovery.

---

### 🩺 Symptom Logger
> *Track what triggers you.*

Log breathing difficulty, coughing, wheezing, chest tightness, and environmental triggers with timestamps. Over time, patterns emerge — certain weather conditions, locations, times of day, or seasons that correlate with your worst days. BreatheSafe makes those patterns visible.

---

### 📊 Analytics Dashboard
> *From data to understanding.*

Built with **D3.js**, the Analytics dashboard shows your comfort score over time, logging streaks, HelpZone episode markers, and symptom progression. It connects the dots between your environment and your health — so you're not just reacting to emergencies, you're anticipating them.

---

## 🏗️ Architecture

```
BreatheSafe/
│
├── index.html                  # Landing page
├── api/                        # Vercel serverless functions
│   ├── weather.js              # Proxies OpenWeather API
│   ├── groq.js                 # Proxies Groq AI API
│   └── maps.js                 # Proxies OSRM routing
│
├── pages/
│   ├── login.html              # Firebase Auth (Google + Email)
│   ├── onboarding.html         # Health profile quiz
│   ├── dashboard.html          # AQI + weather dashboard
│   ├── helpzone.html           # Emergency AI protocol
│   ├── saferoute.html          # Route + AQI map
│   ├── logger.html             # Symptom logging
│   └── analytics.html          # D3.js charts + insights
│
├── js/                         # Feature-specific scripts
├── css/                        # Stylesheets
└── src/                        # Assets, icons, banner
```

**Security model:** All external API keys are hidden behind Vercel serverless functions. The frontend calls `/api/weather` and `/api/groq` — never the external services directly. Firestore security rules enforce per-user data isolation: each user can only read and write their own records.

---

## 🛠️ Tech Stack

| Layer | Technology | Purpose |
|-------|-----------|---------|
| **Frontend** | HTML5, CSS3, Vanilla JS | Core interface |
| **Auth** | Firebase Authentication | Google OAuth + Email/Password |
| **Database** | Cloud Firestore | User data, logs, episodes |
| **AI** | Groq API (llama-3.1-8b-instant) | Emergency protocols + personalized guidance |
| **Routing** | OSRM + Leaflet.js | Real road routes + AQI map overlays |
| **Charts** | D3.js | Analytics and data visualization |
| **Weather/AQI** | OpenWeather API | Live environmental data |
| **Geocoding** | OpenWeather API + Browser Geolocation | Location & coordinate resolution |
| **Backend** | Vercel Serverless Functions | API key proxying |
| **Hosting** | Vercel | Deployment + edge delivery |

---

## 🚀 Getting Started

### Prerequisites
- A modern browser (Chrome, Firefox, Safari, Edge)
- [VS Code](https://code.visualstudio.com/) + [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) (recommended for local dev)
- A Vercel account (for full API functionality)

### Local Development

```bash
# 1. Clone the repository
git clone https://github.com/iammissmiller/BreatheSafe.git

# 2. Navigate into the project
cd BreatheSafe

# 3. Open with VS Code
code .

# 4. Run with Live Server
# Right-click index.html → "Open with Live Server"
```

> **Note:** The `/api/*` serverless functions only run on Vercel. In local development, the app gracefully falls back to localStorage-based data for features that require API calls. To run the full stack locally, use the [Vercel CLI](https://vercel.com/docs/cli): `vercel dev`.

### Deploy Your Own Instance

```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel

# Set environment variables in Vercel dashboard:
# OPENWEATHER_API_KEY
# GROQ_API_KEY
# FIREBASE_* (project config)
```

---

## 🔮 The Roadmap — Making It WAY Better

This is not a finished product. It is a foundation. Here is exactly how BreatheSafe evolves — technically, emotionally, visually, and in impact:

### 🧠 Intelligence Layer
- **Predictive alerts** — ML model trained on your personal symptom + AQI history to predict bad days 24–48 hours in advance
- **Pattern analysis** — automatic detection of your personal triggers (time of day, season, AQI thresholds, weather combinations)
- **Adaptive protocols** — HelpZone action plans that learn from what worked for *you* specifically in past episodes
- **Voice-guided HelpZone** — hands-free breathing instructions during a crisis, because typing is hard when you can't breathe

### 📡 Data & Sensors
- **Wearable integration** — connect with Fitbit, Apple Watch, Garmin for real O₂ saturation, heart rate, and breathing rate data
- **Hyperlocal AQI** — aggregate community sensor data (PurpleAir, OpenSense) for street-level accuracy beyond weather station averages
- **Indoor AQI support** — compatible with smart home sensors (Awair, IQAir) for tracking indoor vs. outdoor air quality comparison
- **Pollen, mold & wildfire overlay** — additional allergen layers on the map for more complete environmental context

### 🗺️ SafeRoute Evolution
- **Real-time rerouting** — automatic alert and alternate route suggestion when AQI spikes mid-journey
- **Saved safe corridors** — mark your personally verified clean walking routes for commutes
- **Public transport integration** — factor in time spent outdoors at stops when comparing routes
- **Community-sourced hazards** — users flag localized pollution events (construction, fires, industrial discharge)

### 🏥 Clinical & Accessibility Bridge
- **Doctor-ready PDF export** — export your symptom log + analytics as a structured report your pulmonologist can actually use
- **Medication reminder system** — log your inhalers, receive smart reminders timed to high-AQI forecasts
- **Emergency contact alerts** — automatically notify a trusted person when a HelpZone episode is triggered
- **Multilingual support** — breathing emergencies happen regardless of language; 10+ language rollout planned
- **Full WCAG 2.1 AA compliance** — screen reader support, keyboard navigation, high contrast mode

### 🎨 Visual & Emotional Evolution
- **Ambient breathing mode** — a full-screen, guided visual breathing exercise with animated rhythm synchronized to recommended breathing counts
- **Calm UI states** — weather-adaptive color themes (clear sky blues on good days, warm ambers on moderate days, muted grays on hazardous ones)
- **Personalized avatar & comfort score** — a gentle visual representation of your respiratory health that evolves with your data
- **Micro-animations** — every interaction should feel alive, calm, and reassuring — never clinical or alarming

### 🌐 Community & Scale
- **Community AQI map** — crowdsourced "I'm feeling fine / struggling today" pins layered over official data
- **School & workplace mode** — group dashboards for organizations to monitor and act on air quality for vulnerable populations
- **PWA & offline mode** — installable as a progressive web app with cached emergency protocols available offline
- **iOS & Android native apps** — built with React Native for push notifications, background location monitoring, and native health kit integration

---

## 🤝 Contributing

BreatheSafe is open source and contributions are genuinely welcome. If you've ever struggled to breathe, or know someone who has, you understand why this matters.

### How to Contribute

```bash
# 1. Fork the repository
# Click "Fork" on GitHub

# 2. Clone your fork
git clone https://github.com/YOUR_USERNAME/BreatheSafe.git

# 3. Create a feature branch
git checkout -b feature/your-feature-name

# 4. Make your changes
# Write clean, commented code
# Test across Chrome, Firefox, and Safari

# 5. Commit with a clear message
git commit -m "feat: add offline fallback for HelpZone protocols"

# 6. Push your branch
git push origin feature/your-feature-name

# 7. Open a Pull Request
# Describe what you changed and why
```

### Good First Issues
- Improve accessibility (ARIA labels, keyboard navigation)
- Add more symptom types to the logger
- Translate UI strings to another language
- Write unit tests for the AQI calculation logic
- Improve mobile responsiveness on small screens
- Add dark mode toggle

### Contribution Guidelines
- Keep the emotional tone of the UI: warm, calm, human — not clinical
- All API keys must go through serverless functions, never client-side
- Test with users who actually have respiratory conditions when possible
- Write code that a beginner can read and understand

---

## 📖 Open Source Programs

BreatheSafe is beginner-friendly and welcomes contributors through:

- **Hacktoberfest** — October contributions eligible for Hacktoberfest rewards
- **GirlScript Summer of Code (GSSoC)** — Open to mentorship collaboration
- **Open Source Connect** — Community-driven development cycles

If you are running an open source program and would like to include BreatheSafe, reach out through [GitHub Issues](https://github.com/iammissmiller/BreatheSafe/issues).

---

## 🔐 Privacy & Security

- **No health data is sold or shared.** Ever.
- All user data in Firestore is scoped strictly per-user via security rules.
- API keys are server-side only via Vercel serverless functions.
- Location data is used only in-session for AQI lookup and routing — never stored persistently.
- All authentication is handled through Firebase (Google-managed infrastructure).

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

You are free to use, modify, and distribute this project. If you build something with it, a mention or star ⭐ is always appreciated.

---

## 👤 Author

**Praptee Miller**

Built with deep care for the 300+ million people living with respiratory conditions who deserve better tools than what exists today.

[![GitHub](https://img.shields.io/badge/GitHub-iammissmiller-1D9E75?style=flat-square&logo=github&logoColor=white)](https://github.com/iammissmiller)

---

## 💛 Support the Project

If BreatheSafe resonated with you:

- ⭐ **Star the repository** — it helps more people discover the project
- 🍴 **Fork it** — build your own version or contribute improvements
- 🐛 **Report bugs** — open an [issue](https://github.com/iammissmiller/BreatheSafe/issues)
- 💬 **Share feedback** — what would make this genuinely useful for you or someone you love?
- 🌍 **Share it** — if you know someone who struggles to breathe, this might help them right now

---

<div align="center">

**BreatheSafe exists so that no one faces a breathing crisis alone, uninformed, or unprepared.**

*We believe respiratory safety should be as accessible as checking the weather.*

<br/>

[![Visit BreatheSafe](https://img.shields.io/badge/Visit%20BreatheSafe-breathe--safe--jet.vercel.app-1D9E75?style=for-the-badge&logo=vercel&logoColor=white)](https://breathe-safe-jet.vercel.app)

<br/>

Made with 💚 by [Praptee Miller](https://github.com/iammissmiller)

</div>
