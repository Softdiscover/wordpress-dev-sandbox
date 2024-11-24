# WordPress Dev Sandbox

A lightweight and flexible development environment for WordPress, powered by Docker. Perfect for testing and developing themes, plugins, or custom WordPress setups.

---

## Features

- Easily configurable with `.env` file.
- Dockerized environment for consistent development and testing.
- Quick setup to get started immediately.

---

## Getting Started

### Step 1: Set up the environment variables
Generate the `.env` file from the example provided:
```bash
cp .env.example .env
```

build docker
```bash
docker compose build
```

run containers
```bash
docker compose up -d
```

after running, add file permissions
```bash
sudo chmod -R g+rw www
```

For debugging, use next chrome extension for enable and disable debug mode: 
https://chromewebstore.google.com/detail/xdebug-chrome-extension/oiofkammbajfehgpleginfomeppgnglk?hl=en

if you don't use that extension, you will get next warning on debug log: 

```bash 
Xdebug: [Step Debug] Could not connect to debugging client. Tried: 172.17.0.1:9003 (through xdebug.client_host/xdebug.client_port).
```



then visit: wp1.docker.local
