# Fatigue Observer — PWA

A mobile-first Progressive Web App for tracking chronic fatigue, symptoms, and medications.

## Features
- 📝 Fatigue & symptom logging
- 💊 Medication / supplement tracker with daily check-off
- 🕒 Timeline of all events
- 📊 Trends & insights (7 / 30 / 90 day views)
- 🔔 Morning & evening check-in reminders (push notifications)
- 📄 Doctor-ready report export
- 📲 Installable on iOS & Android home screen (PWA)
- ✈️ Works offline

---

## Deploy to Vercel

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/fatigue-observer.git
git push -u origin main
```

### 2. Deploy on Vercel
1. Go to [vercel.com](https://vercel.com) → New Project
2. Import your GitHub repo
3. Framework Preset: **Other**
4. Root Directory: leave as `/`
5. Click **Deploy**

That's it — Vercel will auto-deploy on every `git push`.

---

## Install on phone (user instructions)

### iPhone (iOS)
1. Open the app URL in **Safari**
2. Tap the **Share** button (box with arrow)
3. Tap **"Add to Home Screen"**
4. Tap **Add**

### Android
1. Open the app URL in **Chrome**
2. Tap the **three-dot menu** → **"Add to Home screen"**
3. Tap **Add**

> Android users may also see an automatic "Install app" banner appear.

---

## Enabling Notifications

After installing to home screen:
1. Go to **More** tab (⋯)
2. Tap **Enable reminders**
3. Allow notifications when prompted
4. Set your preferred morning and evening times

---

## File structure
```
fatigue-observer/
├── public/
│   ├── index.html      ← The entire app
│   ├── sw.js           ← Service worker (offline + notifications)
│   ├── manifest.json   ← PWA manifest
│   └── icons/
│       ├── icon-192.png
│       └── icon-512.png
└── vercel.json         ← Vercel routing config
```

---

## Future: App Store / Play Store

### Android (Play Store) — ~2–4 weeks
Use [Bubblewrap](https://github.com/GoogleChromeLabs/bubblewrap) or [PWABuilder](https://www.pwabuilder.com) to wrap as a Trusted Web Activity (TWA).

### iOS (App Store) — ~2–4 months
Wrap with [Capacitor](https://capacitorjs.com) or [Expo](https://expo.dev), then submit via Xcode. Requires Apple Developer account ($99/yr).

Quick start: upload your URL to [pwabuilder.com](https://www.pwabuilder.com) — it generates the Android APK automatically and gives you a starting point for iOS.
