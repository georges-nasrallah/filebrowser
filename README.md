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
## Usage
```bash
docker compose up -d
```
Access the UI at `http://<server-ip>:8095`

Default user: `admin`

> If login fails, check the logs for a randomly generated password:
> ```bash
> docker logs filebrowser
> ```
> Once logged in, change your password from the UI under **Profile Settings**.

## Notes

- Files are served from the path defined in the `volumes` section of `docker-compose.yml`.
  Change `/home/georges-nasrallah` to any directory you want to expose via the UI.
