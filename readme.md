# Docker Databases Templates

A collection of ready-to-use Docker Compose templates for popular local development databases.

## Included databases

- MongoDB
- MySQL
- PostgreSQL
- PostgreSQL + pgAdmin
- Redis + Redis Insight

## Quick usage

From the root of this repo:

```bash
docker compose -f mongodb/docker-compose.yml up -d
# or
docker compose -f mysql/docker-compose.yml up -d
# or
docker compose -f postgresql/docker-compose.yml up -d
# or
docker compose -f postgresql2/docker-compose.yml up -d
# or
docker compose -f redis/docker-compose.yml up -d
```

## Common commands

```bash
docker compose ps
docker compose logs -f
docker compose down
```

## Notes

These files are designed as reusable templates for local development. You can copy any folder and paste it into your own project as needed.

## Learn more

Visit the ChaiaurCode community for more Docker and backend projects.