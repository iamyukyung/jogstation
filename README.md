# JogStation

A jogging music player with live workout stats, rebuilt in plain HTML/CSS/JS from a Framer Studio prototype I made in 2016.

- Swipe up on the bottom bar to open the stats sheet; swipe down (or tap the dimmed player) to close it.
- Four stat pages: running speed (per 10 min), heart rate (per minute), duration, distance. Swipe or use the arrows.
- Numbers update every second from a simulated run.
- The purple button plays and pauses the music. Previous/next swap the album like a record.
- Sound: each album plays an original demo loop synthesized in the browser with the Web Audio API (no audio files). Browsers only allow sound after a tap, so the music starts on your first touch.

The whole app is one file: `index.html` (no build step).

## Run locally

```bash
npm install
npm start          # http://localhost:3000
```

Or just open `index.html` in a browser.

## Deploy (Railway)

Create a new Railway project from this GitHub repo. Railway installs dependencies and runs `npm start`, which serves the folder on the `PORT` Railway provides. Then add a public domain under the service's Settings → Networking.
