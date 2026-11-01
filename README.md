# 🎸 Fretlight
A highly realistic, interactive virtual guitar built for the web and Android. 
Fretlight isn't just a soundboard of pre-recorded audio samples. It uses **Karplus-Strong physical string modeling synthesis** via the WebAudio API to generate guitar strings in real-time. This allows for dynamic muting, variable sustain, pitch bends, body resonance, and real-time amp modeling directly in the browser.
## ✨ Features
- **Realistic Physics & Audio Engine**
  - **Karplus-Strong Synthesis:** Strings decay naturally based on thickness, tension, and simulated body resonance.
  - **Amp & Tone:** Switch between Acoustic, Clean, Crunch, and Lead amps with real-time drive curves and EQ.
  - **Tactile Play:** True multi-touch strum zone. Tap, swipe, or hold strings to trigger realistic whole-step pitch bends.
  
- **Play & Practice**
  - **Chord Library:** Extensive library of open and barre chords (automatically voiced based on your tuning).
  - **Song Practice Mode:** Pick a song (like *Teri Meri Kahani* or *Let It Be*), and the app will guide you through the chord progression in time with the tempo.
  - **Auto-Strum:** Build custom strumming patterns (D U -) and let the engine play the rhythm for you.
- **Rhythm Tools**
  - **Drum Machine:** Built-in backing beats (Rock, Folk, Ballad, Reggae).
  - **Metronome:** Tap-tempo enabled visual and audible metronome.
  - **Looper:** Record your strumming sequences and layer them over a timeline.
- **Smart Setup**
  - **Tunings:** Standard, Drop D, Half-down, Open G, Open D, and DADGAD.
  - **Capo:** Place a virtual capo on any fret up to 9; the engine dynamically shifts pitches and chord voicings.
## 🛠️ Tech Stack
- **Frontend:** React 19, TypeScript, Vite, Tailwind CSS v4.
- **Audio:** Native WebAudio API (Oscillators, BiquadFilters, WaveShapers, Delay/Convolvers).
- **Native Android Wrapper:** Capacitor (with native status bar and haptic feedback plugins).
- **Icons:** Lucide React.
## 🚀 Local Development (Web)
To run the web version locally:
```bash
# 1. Install dependencies
npm install
# 2. Start the Vite development server
npm run dev
# 3. Build for production
npm run build
```
## 📱 Android Build
Fretlight is configured as a fully native Android app via Capacitor, featuring a dark status bar, hardware back-button navigation, and native haptic feedback when plucking strings.
```bash
# Generate icons, build the web bundle, and sync into the Android project
npm run android
# Open in Android Studio to run on a device or build an APK
npm run android:open
```
For full instructions on generating keystores, building release APKs, and sideloading, see [README-ANDROID.md](./README-ANDROID.md).
## 🤫 Easter Egg
Tap the Fretlight logo in the top left **7 times rapidly** to activate 🎸 **SHRED MODE**.
---
*Designed and developed by Yashwath.*
