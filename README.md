# Render Keep Alive

A simple GitHub Actions workflow that periodically sends a request to a Render service to help prevent the service from becoming inactive.

## How It Works

GitHub Actions runs every 10 minutes and sends a request to the configured Render health endpoint.

```text
GitHub Actions
      ↓
Every 10 minutes
      ↓
HTTP request
      ↓
Render health endpoint
      ↓
Render service responds
