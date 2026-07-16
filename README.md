# Streak

A one-input arcade game. A glowing orb hurtles through a neon corridor; you thread the gaps, build your streak, and don't touch the walls. Two control modes, switchable on the start and game-over screens:

- **Drag** (default, forgiving): hold and drag up or down to steer the orb proportionally — near the middle is fine control, near the edges is a strong pull. Let go for a gentle, predictable fall.
- **Tap** (twitchy classic): tap anywhere and gravity **inverts**, sending the orb accelerating the other way. Pure momentum, no floatiness.

## How to play

- **Drag mode:** hold and drag up/down to steer (mouse-drag or Arrow/WASD on desktop).
- **Tap mode:** tap anywhere (or Space on desktop) to flip gravity.
- Your choice is saved and remembered next time.
- Slip through each gap to grow your **streak** by one.
- Shave past a gap edge for a **close call** — sparks, a slow-mo beat, and bragging rights on the death screen.
- Every 10 gates the world flashes and the colors heat up. You are on fire. Act accordingly.
- Hit a wall: the orb shatters, you see **STREAK / BEST**, and one tap puts you instantly back in. One more try. Always one more try.

Difficulty ramps smoothly — scroll speed climbs, gaps tighten, and gates land closer together the longer you survive. The first ten gates are forgiving on purpose.

Your best streak is saved on-device (localStorage). All sound is synthesized live with WebAudio — no audio files, no assets, no network.

## What this is

A [Shoebox](https://github.com/rubberduckinspace) bundle: a single `index.html` with inline CSS/JS, no build step, no external libraries, no permissions. It runs in the Shoebox host's locked-down WebView — or in any browser.

Part of the **`arcade-shoebox`** community: tag your game repo `shoebox-app` + `arcade-shoebox` and it appears on the arcade Shelf alongside everyone else's.

## Run it

- On your phone: add `https://rubberduckinspace.github.io/app-streak/` in the Shoebox host.
- Locally: `python3 -m http.server` in this directory, then open `http://localhost:8000`.

## Make it yours

The whole game is one file, and every knob is a small pure function near the top of the script: `speedFor`, `gapHalfFor`, `spacingFor`, `maxCenterShift`. Make it faster. Make the gaps cruel. Change the palette, the particle counts, the near-miss threshold. Ship your own impossible mode.

## Add to Shoebox

Have the Shoebox host installed? Scan this with your **phone's camera or Google Lens** — Shoebox opens with this game pre-filled, ready to add. No typing, no app store. (Your phone's camera does the scanning; Shoebox never asks for a camera permission.)

![Add to Shoebox](add-qr.png)

Or paste the base URL into Shoebox's **+ → Add**: `https://rubberduckinspace.github.io/app-streak/`

Fork it. Change one thing. Push. Watch your phone.
