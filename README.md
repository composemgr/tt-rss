## 👋 Welcome to tt-rss 🚀

Web-based news feed (RSS/Atom) reader and aggregator

## 📋 Description

Web-based news feed (RSS/Atom) reader and aggregator

## 🚀 Services

- **tt-rss**: cthulhoo/ttrss-fpm-pgsql-static:latest

### Infrastructure Components

- **tt-rss-db**: Postgres database


## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/tt-rss/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/tt-rss" ~/.local/srv/docker/tt-rss
cd ~/.local/srv/docker/tt-rss
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install tt-rss
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:8082

## 📂 Volumes

- `./volumes/data/tt-rss` - Data storage
- `./volumes/config/tt-rss` - Data storage
- `./volumes/data/db/postgres/tt-rss` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f tt-rss
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
