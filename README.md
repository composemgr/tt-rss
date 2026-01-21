# Tt Rss

A self-hosted tt-rss application.

## Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/tt-rss/main/docker-compose.yaml" | docker compose -f - up -d
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

## Configuration

See docker-compose.yaml for environment variables and configuration options.

## Documentation

Check the official project documentation for detailed setup and usage information.
