# insta — Simple Chat

A minimal real-time chat built with **Express** + **Socket.IO**. Pick a name,
open it in a couple of browser tabs (or different devices), and messages appear
everywhere instantly. No database, no accounts.

## What it is

Despite the name, this is a lightweight chat demo ("My Chat App"). The front end
lives in `public/`; the server in `server.js`.

## How to run

Requires [Node.js](https://nodejs.org) installed.

```bash
npm install
npm start
```

Then open **http://localhost:3000** in your browser (open a second tab to see both
users talking to each other).

### Chat with someone (same Wi-Fi)

1. Start the server on one machine.
2. Find its local IP (`ifconfig`, `ip addr`, or `ipconfig`), e.g. `192.168.1.50`.
3. The other person opens `http://192.168.1.50:3000` on their device.
4. Everyone picks a name and chats in real time.

## Files

| File | Purpose |
|---|---|
| `server.js` | Express + Socket.IO server; serves `public/` and broadcasts messages |
| `public/index.html` | Chat page (name selector + message list + send box) |
| `public/script.js` | Socket.IO client — sends and renders messages |
| `public/style.css` | Styles |

## Notes

- Messages are not stored — once the page reloads they're gone (live broadcast only).
- Not encrypted — fine for trusted/private use, not for public deployments.