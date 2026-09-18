# Just Us — upgraded foundation

This package starts from your uploaded `Just-us--main` project and upgrades the UI into a mobile-first Just Us foundation.

## Included now
- Magical first opening / notice flow
- Private room-code UI
- Mobile-first home screen
- Chat UI with emoji tray
- Moments/photo capture preview + captions
- Voice/video call screens
- Ludo/Carrom entry screens
- Privacy/E2EE architecture explanation
- Haptic feedback where supported
- Best-effort screenshot/focus notification (not universal browser screenshot detection)
- Original project preserved as `index.original.html`

## Important
The interface is **not yet a production backend**. Do not describe it as fully end-to-end encrypted until the client-side cryptography, authenticated key exchange, secure storage, signaling, access rules, and threat model have been implemented and tested.

## Next production wiring
1. Firebase/Supabase/Cloudflare backend for pairing, presence and signaling.
2. Client-side E2EE using Web Crypto and authenticated key exchange. Never use the room code itself as an encryption key.
3. WebRTC with STUN/TURN for calls.
4. Encrypted photo upload/storage.
5. Server-validated synchronized Ludo and Carrom state.
6. Android native companion app for the true home-screen photo widget. iOS widget support can be added separately.
7. Push notifications and device registration.
8. Security testing before real private data is used.
