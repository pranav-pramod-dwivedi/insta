<p align="center">
  <img src="assets/cover.svg" width="830" alt="insta cover" />
</p>

<h1 align="center">insta</h1>

<p align="center">
  A tiny real-time chat that just works.<br/>
  No server, no cloud. Don't let the name fool you — there are no feeds or influencers.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/stack-HTML%20%2B%20JS%20%2B%20PeerJS-833ab4" alt="stack" />
  <img src="https://img.shields.io/badge/host-GitHub%20Pages-24292e" alt="host" />
</p>

## Try it live

https://pranav-pramod-dwivedi.github.io/insta/

Pick a name, create a room, send the invite. Messages go straight between browsers —
no server, no database, nothing stored anywhere.

## How it works

- Pick a name (Pranav, Naman, whoever).
- **Create room** gives you a 5-letter code and an invite link.
- Anyone with the link joins and every message shows up live for the room.
- It runs **peer to peer** over PeerJS, so it lives for free on GitHub Pages like a plain static page.

## Run it locally

```bash
python3 -m http.server 8000   # from this folder → http://localhost:8000
```

Same Wi-Fi? Open `http://<your-LAN-IP>:8000`. One creates a room, the rest join.
No npm, no install.

## Notes

- It isn't Instagram. It's a one-trick chat demo and it knows it.
- Chat rides PeerJS's free public broker. Broker naps, chat naps.
- Not encrypted. Fine for friends, not for secrets.
- Invite links auto-point at wherever the page is hosted, so they just work.

<p align="center">made for the "brb, testing something" energy</p>