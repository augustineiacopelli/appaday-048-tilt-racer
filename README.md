# 048 — Tilt Racer

**AppADay** · Day 048 · June 24, 2026 · Category: G (Games)

[▶ Play Live](https://augustineiacopelli.github.io/appaday-048-tilt-racer/) · [◀ Full Portfolio](https://augustineiacopelli.github.io/appaday/)

-----

## What It Does

A 3D arcade racer you steer by physically tilting your device. Dodge oncoming traffic on a neon-lit asphalt track as speed climbs relentlessly toward the limit. Every car you dodge scores points; the road never lets up. Survive as long as you can.

## Controls

|Input                   |Action                  |
|------------------------|------------------------|
|Tilt device left / right|Steer                   |
|Arrow keys or A / D     |Steer (desktop fallback)|


> **iOS note:** On first launch, tap **START ENGINE** to grant motion permission. This is required by Safari for `DeviceOrientationEvent` access.

## How It Works

- Built with [Three.js r128](https://threejs.org/) for 3D rendering — single CDN import, no build step
- `DeviceOrientationEvent.gamma` drives lateral steering with a `requestPermission()` gate for iOS 13+
- Traffic spawns in three lanes at increasing frequency as speed climbs
- Camera shake activates above 55 speed units for physical feedback
- High score persisted in `localStorage`

## Tech

Single-file vanilla HTML/CSS/JS. No frameworks, no build tools. Deploys as a static file to GitHub Pages.

-----

*Part of [AppADay](https://augustineiacopelli.github.io/appaday/) — one complete web app built and shipped every day.*
