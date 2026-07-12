# Palworld Server

This stack runs the [`thijsvanloef/palworld-server-docker`](https://github.com/thijsvanloef/palworld-server-docker) image with Discord webhook notifications wired through an env file.

## Setup

1. Copy `.env.example` to `.env`.
2. Set `DISCORD_WEBHOOK_URL` in `.env`.
3. Start the stack with Docker Compose.

```bash
docker compose up -d
```

The compose file reads the webhook URL from `.env` and reuses it for all Discord notification endpoints.
