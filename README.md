# Filebrowser

A self-hosted file browser accessible via web UI.

## Requirements

- Docker & Docker Compose
- Either export the variables in your `.bashrc`:
```bash
export PUID=1000
export PGID=1000
```
> Run `id` to get your actual UID and GID.

- Or create a `.env` file next to your `docker-compose.yml`:
```env
PUID=1000
PGID=1000
```
