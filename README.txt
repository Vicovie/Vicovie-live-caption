VICOVIE LIVE CAPTION — PUBLIC BETA 1.1
VICOVIE TECHNOLOGIES
Every Word. Every Song. Every Moment.

WHAT IS INCLUDED
- Live speech-to-text through browser Web Speech Recognition (supported Chrome/Edge versions; availability depends on browser, language and provider).
- Manual captions and correction: click any recent caption to load it into the correction field, edit, then Display.
- Separate projector display with live updates, full-screen support (F11), theme and size controls.
- Church, worship/concert, meeting, conference and presentation modes.
- English (Nigeria/US), Yoruba, Igbo, Hausa and French language selection (actual recognition support varies by browser/provider).
- Recent caption history, word/line counts, TXT transcript and SRT export.
- Installable PWA shell and cached interface files for repeat opening.
- Responsive interface for laptop and mobile browser.

IMPORTANT: WHAT THIS APP DOES NOT YET DO
- Offline AI speech transcription. The interface may open from cache offline, but speech recognition normally requires internet and a supported browser speech service.
- Automatic song identification or automatic song lyrics.
- Automatic translation. Selecting a language changes the recognition language; it does not translate.
- Phone-as-remote-control / remote operator connection across devices.
- Direct vMix or OBS overlay/plugin integration.
- Native Android APK or Windows installer. This release is an installable web app (PWA) where the browser supports installation.

RUN LOCALLY ON A LAPTOP
1. Extract this ZIP.
2. Open a terminal in the vicovie-live-caption folder.
3. Run: python -m http.server 8000
4. Open Chrome or Edge at http://localhost:8000
5. Allow microphone permission.
6. Set the church USB audio interface/mixer feed as the laptop's default input in operating-system sound settings.
7. Start microphone, open projector, move projector window to the TV/projector screen and press F11.

PUBLIC HOSTING / GOING LIVE
This ZIP is ready to deploy as a static HTTPS website. To publish it, upload the contents of the vicovie-live-caption folder to a static hosting provider such as Netlify Drop, Cloudflare Pages or GitHub Pages. The published address must use HTTPS for microphone permission. A public domain, hosting account and deployment approval are controlled by the owner; this package does not itself create a public website or hosting account. After publishing, test on the actual church laptop and mixer before announcing it to churches.

CHURCH AUDIO SETUP
- Use a clean AUX/REC/USB output from the mixer into a suitable USB audio interface/sound card.
- Select that interface as the laptop's default input before opening the app. The browser SpeechRecognition API does not offer consistent per-device input selection in all browsers.
- Start with conservative input gain and test the pastor and choir separately.
- Never connect a power-amplifier speaker output directly to a laptop or interface input.

PRIVACY & RELIABILITY
- The app's own code does not record or save raw audio. Browser speech recognition may process audio through the browser/provider service; churches should review the provider's privacy terms and obtain any required consent.
- Captions are held in the active browser session/local display state; download the transcript before closing if you need a record.
- Recognition can mishear names, scripture references, accents, music and overlapping voices. A human operator should correct captions.
- Do not rely on this beta as the only accessibility or broadcast caption system. Keep manual captions or a backup presentation ready.

BEFORE A LIVE SERVICE
[ ] Open the HTTPS website in Chrome/Edge.
[ ] Allow microphone permission.
[ ] Confirm the mixer/interface is the selected system input.
[ ] Test pastor speech and choir separately.
[ ] Open projector display and verify on the actual TV/projector.
[ ] Check font size, contrast, line readability and manual correction.
[ ] Confirm stable internet and test recognition service availability.
[ ] Download a test transcript and keep a manual backup.

RELEASE STATUS
Public Beta 1.1 — deployment-ready package, not yet publicly hosted or independently certified. Offline AI, automatic song identification/lyrics, phone remote control, and vMix/OBS integration are future features.
