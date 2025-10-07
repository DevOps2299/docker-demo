# My Nginx + Uptime Kuma Docker Setup

This project sets up a simple **Nginx web server** and an **Uptime Kuma monitoring dashboard** using Docker Compose.

---

## 🧩 Services

### 1. Nginx (`web`)
- Builds a custom Nginx image from the included `Dockerfile`
- Exposes port **8080** on the host (mapped to port **80** inside the container)
- Automatically restarts unless manually stopped

### 2. Uptime Kuma (`uptime-kuma`)
- Uses the official [louislam/uptime-kuma](https://hub.docker.com/r/louislam/uptime-kuma) image
- Provides an uptime and performance monitoring dashboard
- Stores configuration and data locally in `uptime-kuma-data/`
- Accessible on port **3001**

---

## 🚀 Getting Started

### 1. Build and start the containers
```bash
docker compose up -d
