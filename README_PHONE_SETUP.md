# JARVIS Mobile Prototype 0.2

This project is a phone-first Progressive Web App (PWA). It can be opened on Android in a browser and, when hosted over HTTPS, installed using the browser's **Add to Home screen** / **Install app** option.

## Included
- Futuristic dark-blue JARVIS dashboard
- Tap-to-talk speech recognition when supported by the browser/device
- Spoken replies using browser text-to-speech
- Text chat interface
- Local demo commands: greeting, time, date, help
- Basic offline cache after first successful load

## Honest limitations
This is not a full AI assistant yet. It does not connect to an AI model, continuously listen for a wake word, or control Android system settings. Browser speech recognition support varies by browser and may use an online speech service. The app only listens after the user taps the microphone.

## Use it without a computer
1. Extract the ZIP on your Android phone using Files or another archive app.
2. To make it installable, the folder must be hosted on an HTTPS static host. One phone-only route is to create a repository using GitHub's mobile website, upload the files while preserving their folders, then enable GitHub Pages in repository Settings > Pages.
3. Open the resulting HTTPS Pages address in Chrome on Android.
4. Open Chrome's three-dot menu and choose **Install app** or **Add to Home screen**.
5. Allow microphone permission when asked.

You can also open `index.html` locally to preview the interface, but local-file mode may not support microphone access, offline installation, or service workers.

## AI upgrade
For genuine open-ended AI answers, connect a small HTTPS backend that stores the AI provider credential securely and relays chat requests. Do not publish API keys in this static app or repository. A hosted backend and provider account may have usage costs.
