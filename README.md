# Golf Plan

Personal Android app for the 26-week home golf fitness plan (23 Nov 2026 – 23 May 2027).

- Week and day tabs with every session, exercise descriptions and sets × reps
- Tick off exercises; progress is saved on the phone (app storage, kept across updates)
- "Continue where I left off" jumps to the next unfinished session
- Back up / restore progress as text (share to Notes, email, Drive)

## Install / update
1. Open the latest release under **Releases** on your phone.
2. Download `GolfPlan-N.apk` and open it. Allow installing from your browser if Android asks.
3. Newer builds install over the old one and keep your progress (same signing key every build).

## Editing the plan
The whole schedule lives in `app/src/main/assets/index.html` (the `EX` exercise library and the `session*` functions). Push to `main` and GitHub builds a new APK.

Note: `keystore.b64` is the app's signing key, committed on purpose so every build can update the installed app. Keep this repository private.
