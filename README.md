# readmission

For managing Redis databases, like PHPMyAdmin.

## How to use

In Dockerfile, write:

```yaml
services:
  readmission:
    image: tarsislimadev/readmission
    ports:
      - 8000:8000
    depends_on:
      - redis
  redis:
    image: redis:alpine
    ports:
      - 6379:6379
```

Run in bash:

```bash
docker compose up -d
```

Open in browser

[localhost:8000](http://localhost:8000)

## license

[MIT](./LICENSE)
