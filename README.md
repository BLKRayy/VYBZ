# VYBZ
🎵 VYBZ — TikTok & Meme Soundboard

The ultimate browser-based soundboard featuring viral TikTok song vibes + iconic internet meme sounds. Zero dependencies. Zero audio files. Pure Web Audio API.

🔊 Sound Library
🎵 TikTok Songs (Procedural vibes)
SoundKeyInspired ByEspresso DropQSabrina Carpenter – bouncy pop hookBirds of a FeatherWBillie Eilish – dreamy arpeggioDie With a SmileEBruno Mars x Lady Gaga – power chordNot Like UsRKendrick Lamar – trap beat dropMillion $ BabyTTommy Richman – funky grooveANXIETYYDoechii – stuttery energy (51.6B views)Pretty Little BabyAConnie Francis – retro doo-wop revivalEnd of BeginningSDjo – melancholic indie waveNastyDTinashe – sultry R&B groove
😂 Meme Sounds
SoundKeyOriginBRUHFUniversal reaction tromboneOOFGRoblox death soundSad TromboneHWah wah wahhhhAIRHORNJHype machinePEW PEWKLaser edit kingRizz AlertLW rizz detectedVine BoomZSub bass impactEmotional DamageXSteven He classicNPC ModeCTikTok NPC streamLow Taper FadeV2024 haircut memeDing Dong Eat It UpBMost chaotic 2024 meme
⚡ Sound FX
SoundKeyUseNotificationNSocial pingTape RecordMRecord buttonGlitch,Signal errorLevel Up.AchievementBig Boom—CinematicKa-Ching/Money SFX

✨ Features

🎛️ Real-time Volume, Reverb & Pitch controls
⌨️ Full keyboard shortcuts (see table above)
🌈 Live 64-bar frequency visualizer
🏷️ Category filters — TikTok / Memes / SFX
💫 Ripple click animations + glow effects
📱 Fully responsive mobile layout
🎚️ Pitch shifter — make any sound cursed
🔔 Now Playing indicator overlay
🚫 Zero audio files — all synthesized in real-time


📁 File Structure
vybz/
├── index.html              ← Entire app (single file, ~600 lines)
├── README.md               ← This file
├── LICENSE                 ← MIT
└── .github/
    └── workflows/
        └── deploy.yml      ← Auto GitHub Pages deploy


🧠 How the Audio Works
Everything is synthesized using the Web Audio API:
OscillatorNode → BiquadFilter → GainNode → MasterGain
                                               ↓
                               DryGain ←── MasterGain ──→ WetGain
                                  ↓                           ↓
                              AnalyserNode ←── ConvolverNode (reverb)
                                  ↓
                           AudioDestination

Oscillators – sine, triangle, sawtooth, square waves
Gain envelopes – ADSR-style attack/decay/sustain/release
BiquadFilter – highpass/lowpass/bandpass for tone shaping
ConvolverNode – impulse response reverb (procedurally generated)
AnalyserNode – FFT data fed to the visualizer canvas
BufferSourceNode – white noise synthesis for percussive hits


📜 License
MIT © 2025 VYBZ — Fork it, remix it, make it go viral.
