# MySQL Local Template

This folder contains a ready-to-use MySQL setup for local development.

## Start the container

```bash
docker compose up -d
```

If you are starting it from the repo root:

```bash
docker compose -f mysql/docker-compose.yml up -d
```

## Access Adminer

Open:

```bash
http://localhost:8080
```

Login details:

- System: `MySQL`
- Server: `db`
- Username: `chai`
- Password: `chai`
- Database: `chaiDB`

## Access MySQL shell

```bash
docker compose exec db mysql -u chai -p chaiDB
```

## Stop and remove containers

```bash
docker compose down
```

## Useful notes

- The database is stored in a named Docker volume for persistence.
- This template is designed to be reusable in personal projects.
