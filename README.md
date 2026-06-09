<div align="center">

<img src="https://github.com/iammissmiller/BreatheSafe/blob/main/src/banner.png?raw=true" alt="BreatheSafe Banner" width="100%"/>

<br/>
<br/>

[![Live Demo](https://img.shields.io/badge/Live%20Demo-breathe--safe--jet.vercel.app-1D9E75?style=for-the-badge&logo=vercel&logoColor=white)](https://breathe-safe-jet.vercel.app)
[![HackIndia](https://img.shields.io/badge/HackIndia-Vibe%20Coding%202026-EA580C?style=for-the-badge)](https://hackindia.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-0F6E56?style=for-the-badge)](LICENSE)

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://github.com/iammissmiller/BreatheSafe)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://github.com/iammissmiller/BreatheSafe)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://github.com/iammissmiller/BreatheSafe)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)](https://firebase.google.com)
[![Groq](https://img.shields.io/badge/AI-Groq-FF4B00?style=flat-square)](https://groq.com)
[![Vercel](https://img.shields.io/badge/Deployed%20on-Vercel-000?style=flat-square&logo=vercel)](https://vercel.com)

<br/>

> *Every breath should feel safe.*
>
> An AI-powered respiratory health platform that monitors your air, guides you through breathing emergencies,
> and gives you personalized health intelligence — in real time, wherever you are.

<br/>

</div>

---

## 💡 The Problem

I have breathing issues. Traveling, pollution, unexpected triggers — and in those moments of panic, I had no idea what to do or where to go.

That's why I built BreatheSafe.

Over **300 million people** live with asthma. Hundreds of millions more deal with air pollution daily — stepping outside into air that triggers symptoms they can't measure, facing breathing emergencies with no real-time guidance, and finding tools that are either too clinical, too generic, or too slow.

**BreatheSafe fills that gap** — combining live air quality data, AI emergency guidance, safe route navigation, and personal health tracking into one accessible browser app.

---

## 🤖 Built with Vibe Coding

This project was built using **Claude** and **ChatGPT** as the core AI development tools — prompting components into existence, debugging logic, designing architecture, and iterating on features rapidly.

The entire workflow was AI-first: describe the feature in plain English → prompt → refine → ship. No boilerplate written by hand. True vibe coding from idea to product.

| AI Tool | How It Was Used |
|---------|----------------|
| **Claude** | Architecture design, component logic, API integration, debugging |
| **ChatGPT** | UI ideation, feature brainstorming, copy and content |

---

## ✨ Features

### 🆘 HelpZone — AI Emergency Protocol
Select your symptoms — asthma attack, hyperventilation, dust exposure — and HelpZone generates a **timed, step-by-step AI action plan** personalized to your health profile and current environment. Every episode is saved to Analytics.

### 🌫️ Air Quality Dashboard
Live AQI, PM2.5, humidity, wind speed, and UV index from your exact GPS coordinates. Color-coded severity indicators and personalized health alerts based on your respiratory profile.

### 🗺️ SafeRoute — Pollution-Aware Navigation
Find the nearest hospital or safe location during a breathing emergency. Powered by **OSRM + Leaflet.js** with live AQI overlays on real road routes.

### 📊 Analytics Dashboard
**D3.js** powered charts showing your comfort trends, logging streaks, episode history, and symptom patterns over time.

### 🩺 Symptom Logger
Log breathing difficulty, coughing, wheezing, and environmental triggers with timestamps. Patterns emerge — BreatheSafe makes them visible.

### 🔐 Secure Auth
Firebase Authentication with Google OAuth and Email/Password. Firestore security rules ensure each user's data is fully private.

---

## 🏗️ Architecture & Tech Stack

```
BreatheSafe/
│
├── index.html                  # Landing page
├── api/                        # Vercel serverless functions (API key proxying)
│   ├── weather.js              # OpenWeather API proxy
│   └── groq.js                 # Groq AI proxy
│
├── pages/                      # Dashboard, HelpZone, SafeRoute, Analytics, Login
├── js/                         # Feature scripts
├── css/                        # Stylesheets
└── src/                        # Assets & icons
```

| Layer | Technology |
|-------|-----------|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| Auth | Firebase Authentication |
| Database | Cloud Firestore |
| AI | Groq API (llama-3.1-8b-instant) |
| Routing & Maps | OSRM + Leaflet.js |
| Charts | D3.js |
| Weather & AQI | OpenWeather API |
| Backend | Vercel Serverless Functions |
| Hosting | Vercel |

**Security:** All API keys are hidden behind Vercel serverless functions. The frontend never calls external APIs directly. Firestore rules enforce strict per-user data isolation.

---

## 🔮 Future Roadmap

- 📱 Native Android & iOS app (React Native)
- 🚨 Emergency SOS — one-tap alerts to emergency contacts
- 🧠 Predictive alerts — ML model trained on personal symptom + AQI history
- 🏥 Nearby hospital & pharmacy finder
- 📄 Doctor-ready PDF export of symptom logs
- 🌍 Multi-language support
- 📡 Wearable integration (Apple Watch, Fitbit) for real O₂ data
- 🔔 Push notifications for AQI spikes

---

## 👥 Team — BreakOut-Zone

| Name | Role |
|------|------|
| Praptee Miller | Developer & Designer |
| Prashant Kumar Sahu | Testing |

---

## 🌐 Live Site

**[breathe-safe-jet.vercel.app](https://breathe-safe-jet.vercel.app)**

---

## 📄 License

MIT License

---

<div align="center">

**BreatheSafe exists so that no one faces a breathing crisis alone, uninformed, or unprepared.**

<br/>

[![Visit BreatheSafe](https://img.shields.io/badge/Visit%20BreatheSafe-breathe--safe--jet.vercel.app-1D9E75?style=for-the-badge&logo=vercel&logoColor=white)](https://breathe-safe-jet.vercel.app)

<br/>

Made with 💚 by [Praptee Miller](https://github.com/iammissmiller)

</div>
