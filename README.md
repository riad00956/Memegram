# Memegram

A premium Telegram Bot messenger application built with React + Vite, convertible to Android APK using Capacitor.

## Features

- 📱 Telegram Bot integration
- 💬 Real-time messaging
- 🌙 Dark mode support
- 🎨 Customizable theme colors
- 📷 Media sharing (photos, videos, documents)
- 🔒 Chat blocking
- 👥 Multiple bot support (up to 3)

## Tech Stack

- **Frontend**: React 19 + TypeScript + Vite
- **Styling**: Tailwind CSS v4 + Radix UI
- **Mobile**: Capacitor.js (Android APK)
- **Animations**: Framer Motion

## Development

```bash
npm install
npm run dev
```

## Build Web App

```bash
npm run build
```

## Build Android APK

### GitHub Actions (Automatic)

Push to `main` branch → GitHub Actions will automatically build the APK.  
Download APK from **Actions → Build Android APK → Artifacts → memegram-debug-apk**

### Manual Build (Local)

Prerequisites: Node.js 20+, Java 17+, Android SDK

```bash
# Install dependencies
npm install

# Build web
npm run build

# Add Android (first time only)
npx cap add android

# Sync
npx cap sync android

# Build APK
cd android && ./gradlew assembleDebug

# APK location:
# android/app/build/outputs/apk/debug/app-debug.apk
```

## Telegram Bot Setup

1. Create a bot via [@BotFather](https://t.me/BotFather)
2. Get your bot token
3. Open the app and enter your token

## Environment Variables

See `.env.example` for required variables.

## License

MIT
