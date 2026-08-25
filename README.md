# Ubuntu FREE VPS — HyperVM Web Console

Ubuntu 24.04-based free VPS web terminal (FastAPI + PTY console), deployable on platforms like Render.

## Requirements
- Env var `CONSOLE_TOKEN` (authentication token for the web console)
- Exposes `PORT` (default: `10000`)

## Build & Run
```bash
docker build -t ubuntu-free-vps .
docker run -d -p 10000:10000 -e CONSOLE_TOKEN=my-secret-token ubuntu-free-vps
```

Then open `http://localhost:10000` in your browser and authenticate with your token.
