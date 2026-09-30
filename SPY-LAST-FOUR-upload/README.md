# SPY: LAST FOUR

A no-login multiplayer hotel mystery game for five or six players.

## Run locally

Requires Node.js 20 or newer.

```sh
npm start
```

Open `http://localhost:3000`. Each player needs the same server address and room code. `localhost` is only reachable from the computer running the server.

## Public preview deployment

This project includes a Render Blueprint in `render.yaml`. To deploy it, push this folder to a Git repository, connect that repository in Render, and create a service from the Blueprint. Render assigns a public `onrender.com` address after the first successful deploy.

The Blueprint selects Render's free web service. Free services can sleep when idle, and this game's room state currently lives in server memory. A service sleep, restart, or deploy therefore ends any active rooms. Use a continuously running instance and persistent room storage before relying on it for uninterrupted public games.
