# ChatNews

Chat with AI about the latest news. Get summaries, deep dives, and answers in a conversational format.

## Development

```bash
# Build backend
cd backend
cargo build --release -p news-server

# Run locally
DATABASE_PATH=./news.db STATIC_DIR=../frontend cargo run -p news-server
```

## Deployment

Deployed to [Fly.io](https://fly.io) via GitHub Actions.

```bash
flyctl deploy
```

## Architecture

- **Backend**: Rust (axum) + SQLite
- **Frontend**: Vanilla JS PWA
- **Deploy**: Fly.io (chatnews-link)
