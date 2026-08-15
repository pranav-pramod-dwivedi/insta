<p align="center">
  <img src="assets/cover.svg" width="830" alt="insta cover" />
</p>

<h1 align="center">insta</h1>

<p align="center">
  A tiny real-time chat that just works.<br/>
  Don't let the name fool you. There are no feeds, no stories, no influencers.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/stack-Node%20%2B%20Express%20%2B%20Socket.io-833ab4" alt="stack" />
  <img src="https://img.shields.io/badge/scope-small%20and%20quick-fd1d1d" alt="scope" />
</p>

Pick a name, open the page, type. Messages show up everywhere that's connected the
moment you hit send. That's the whole app. It's meant to be that small.

## What it does

- A dropdown to set your name (Pranav or Naman).
- Send a message and it broadcasts to every open tab and device.
- Nothing gets saved. Reload the page and it's a fresh room.

## Run it

```bash
npm install
npm start     # → http://localhost:3000
```

To see it do its thing, open a **second tab**, pick the other name, and message
yourself back and forth. I know, deeply sad. It works though.

### Chat with a friend (same Wi-Fi)

1. Run the server on one machine.
2. Get its local IP: `ifconfig | grep inet` or `ipconfig`.
3. Other device opens `http://<that-IP>:3000` and picks a name.

## Files

| File | Job |
|---|---|
| `server.js` | Express + Socket.IO server, serves and broadcasts |
| `public/index.html` | the chat screen |
| `public/script.js` | the client, sends and renders messages |
| `public/style.css` | the looks |

## Notes

Not encrypted. Great for your house, not for the public internet. Use it for the vibe,
not your passwords.

<p align="center">made for the "brb, testing something" energy</p>