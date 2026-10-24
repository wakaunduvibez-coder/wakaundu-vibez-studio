# WakaûndūVibez Studio — Android starter v0.2

## Working features
- Dark studio-style Compose interface
- Built-in offline synthesized Gengetone-inspired drum loop (kick, snare and hi-hat)
- Tempo control from 70–150 BPM (locked while loop is playing)
- Start/stop beat playback using Android `AudioTrack`
- Record vocal takes from the phone microphone to app-private M4A/AAC files
- Play back the most recently recorded take

## Build and run
1. Install Android Studio (use its bundled JDK).
2. Extract this ZIP and open the project folder in Android Studio.
3. Let Gradle sync complete.
4. Connect your Android phone with USB debugging enabled, or use an emulator (a physical phone is best for microphone testing).
5. Press Run and grant microphone permission.
6. In Beat Lab, press **Play beat**. Stop it to change BPM.
7. Use headphones to avoid the beat leaking into your vocal recording.
8. Record and play back your take in Vocal Booth.

## Important limitations
This is an early source-code prototype, not a finished DAW or compiled APK. The beat is a synthesized loop, not a sampled commercial beat. Beat playback and vocal recording are currently separate functions; this version does not yet mix the beat into the recorded vocal file or synchronize multiple tracks. It does not yet include effects, multitrack editing, project saving, mastering, or final song export.

Before public release, build and test on several Android devices, handle audio focus/device routing, and implement the remaining production features.
