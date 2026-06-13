<p align="center">
  <img src="icons/app-icon-180.png" alt="Mood Button app icon" width="128" height="128">
</p>

<h1 align="center">Mood Button / 心情按钮</h1>

<p align="center">
  <strong>Speak once. Get a private mood diary.</strong>
  <br>
  Apple MLX + Qwen3 local AI - voice mood diary - iPhone
  <br>
  <a href="https://hooosberg.github.io/mood-button/">Official Website</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-iOS%2017+-444.svg" alt="iOS 17+">
  <img src="https://img.shields.io/badge/AI-Apple%20MLX%20%2B%20Qwen3-2f6fed.svg" alt="Apple MLX and Qwen3">
  <img src="https://img.shields.io/badge/privacy-local%20first-2e7d32.svg" alt="Local first">
  <img src="https://img.shields.io/badge/IAP-skin%20pack-lightgrey.svg" alt="Optional skin pack">
</p>

<p align="center">
  <a href="https://hooosberg.github.io/mood-button/">
    <img src="media/hamster-heart-home.jpg" alt="Mood Button hamster home screen" width="360">
  </a>
</p>

Mood Button is a small iPhone app for turning a short voice recording into a private mood diary. The core experience is intentionally simple: open the app, hold the mood button, speak naturally, and let the app organize the day into a readable journal entry with mood signals, context, and recall-friendly structure.

The app is built around a local-first AI pipeline. Apple Speech handles transcription, and the diary generation layer runs Qwen3 with Apple MLX on supported physical iPhone devices. The goal is not a social feed or a medical tool. It is a quiet personal notebook that helps you keep track of how a day felt.

## Product Highlights

- Voice-first diary capture: press the mood button and talk instead of typing a blank page from scratch.
- AI-generated diary entries: recordings are organized into a concise journal draft that can be reviewed later.
- Local AI engine: Apple MLX runs a bundled Qwen3 MLX model on supported physical iPhones.
- Mood recognition: the app extracts mood signals and turns them into calendar, curve, and recall views.
- Local review and search: revisit entries by date, mood, keyword, or memory cues.
- Clear privacy boundaries: core diary storage, organization, review, and search stay on the device.
- Optional skins: the hamster theme is the default; extra home skins are planned as a one-time skin pack.

## Privacy At A Glance

| Area | Behavior |
|---|---|
| Account | No account required |
| Diary storage | Stored locally in the app sandbox |
| Local AI | Qwen3 MLX model is bundled with the app |
| Speech transcription | Uses Apple Speech, preferring on-device recognition when available |
| Weather context | Optional; only after Location permission, using rounded location data |
| Tracking | No third-party advertising tracker is used |
| Paid feature | Optional home skins only; core diary features remain available |

Full text: [Privacy Policy](https://hooosberg.github.io/mood-button/privacy.html) · [Terms of Service](https://hooosberg.github.io/mood-button/terms.html)

## Public Links

- Website: <https://hooosberg.github.io/mood-button/>
- Support: <https://hooosberg.github.io/mood-button/support.html>
- Privacy Policy: <https://hooosberg.github.io/mood-button/privacy.html>
- Terms of Service: <https://hooosberg.github.io/mood-button/terms.html>
- Repository: <https://github.com/hooosberg/mood-button>

## Repository Layout

```text
.
|-- index.html              GitHub Pages landing page
|-- support.html            support page for App Store review and users
|-- privacy.html            privacy policy
|-- terms.html              terms of service
|-- i18n.js                 landing-page localization strings
|-- styles.css              site styles
|-- icons/                  public app icon assets
`-- media/                  public home-skin previews
```

## Technical Notes

The iOS app is built with SwiftUI and SwiftData. Recording uses AVFoundation, transcription uses Apple Speech, optional weather context uses Open-Meteo, and diary generation is powered by Apple MLX with a bundled Qwen3 MLX model on supported devices. This public repository contains the GitHub Pages site and App Store-facing public material; the local development workspace keeps the full iOS source and release evidence.

## Developer

Built by [hooosberg](https://github.com/hooosberg).

Contact: [zikedece@proton.me](mailto:zikedece@proton.me)
