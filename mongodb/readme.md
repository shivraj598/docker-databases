# MongoDB Local Template

This folder provides a ready-to-use MongoDB setup for local development.

## Start the container

```bash
docker compose up -d
```

If you are running from the repo root:

```bash
docker compose -f mongodb/docker-compose.yml up -d
```

## Connection details

- Host: `localhost`
- Port: `27017`
- Username: `root`
- Password: `example`

Connection string:

```bash
mongodb://root:example@localhost:27017
```

## Access MongoDB shell

```bash
docker compose exec mongo mongosh -u root -p example --authenticationDatabase admin
```

## Stop and remove containers

```bash
docker compose down
```

## Useful notes

- Data is stored in a named Docker volume so it persists across container restarts.
- This template is meant to be copied into a project when you need a quick local MongoDB setup.
