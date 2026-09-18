# Just Us — upgraded build

This is a single-file mobile-first private-chat prototype based on the uploaded Just Us files.

## What is wired
- WhatsApp-style chat layout.
- Profile photo upload + crop-style circular preview.
- Realtime Firebase Firestore presence and messages.
- Text, emoji and compressed photo messages.
- Online / last-seen presence.
- Voice/video call UI with WebRTC + Firestore signaling.
- Ludo and Carrom playable two-person turn-taking prototypes.
- Game invitation with Accept / Reject.
- 2.5-second animated ancient notice scene.
- Privacy page explaining what is and is not actually end-to-end encrypted.

## Important security
The Firebase web config is not a password. The app is NOT automatically true E2EE. Before using real sensitive data:
1. Enable Firebase Authentication (anonymous or account-based).
2. Replace test-mode Firestore rules with rules that only permit the two authorized participants.
3. Move photo delivery to Firebase Storage with strict rules.
4. Encrypt message/photo payloads on-device with authenticated key exchange.
5. Add a TURN server for reliable calls across restrictive NATs.
6. Test the security rules and threat model.

## Run
Upload `index.html` to GitHub Pages, Firebase Hosting, Netlify, etc. HTTPS is required for camera/microphone access.

The existing Firebase project values from the supplied project were retained so the build can connect to the same project.
