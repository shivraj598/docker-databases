# Redis Local Template

This folder contains a ready-to-use Redis setup with Redis Insight.

## Start the container

```bash
docker compose up -d
```

If you are running it from the repo root:

```bash
docker compose -f redis/docker-compose.yml up -d
```

## Access Redis Insight

Open:

```bash
http://localhost:8001
```

Use the following connection details:

- Host: `redis`
- Port: `6379`

## Access Redis CLI

```bash
docker compose exec redis redis-cli
```

## Stop and remove containers

```bash
docker compose down
```

## Useful notes

- Redis stores data in a named Docker volume.
- Redis Insight is included for easy local monitoring and debugging.
- This setup is useful as a starting point for apps that need a fast in-memory cache or queue.
