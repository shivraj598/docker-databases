# PostgreSQL Local Template

This folder contains a ready-to-use PostgreSQL setup for local development.

## Start the container

```bash
docker compose up -d
```

If you are starting it from the repo root:

```bash
docker compose -f postgresql/docker-compose.yml up -d
```

## Access Adminer

Open:

```bash
http://localhost:8080
```

Login details:

- System: `PostgreSQL`
- Server: `db`
- Username: `chaiaurcode`
- Password: `chaiaurcode`
- Database: `chaiDB`

## Access PostgreSQL shell

```bash
docker compose exec db psql -U chaiaurcode -d chaiDB
```

## Stop and remove containers

```bash
docker compose down
```

## Useful notes

- Data is stored in a named Docker volume for persistence.
- This template is meant to be copied into a project when you want a local PostgreSQL database quickly.
