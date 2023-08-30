# Traefik Boilerplate

This is a boilerplate for setting up a Traefik Proxy with Docker Compose.

It includes a basic configuration to obtain wildcard certificates from Let's Encrypt using Hurricane Electric DNS.

## Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/zlskey/traefik-boilerplate.git

   ```

1. Copy `.env.example` to `.env` and fill in the values

   ```bash
   cat .env.example > .env
   ```

1. Change `mail@example.com` to your email address in `traefik.yml`

1. Create a `proxy` network

   ```bash
   docker network create proxy
   ```

1. Run

   ```bash
   docker-compose up -d
   ```

Admin panel is available at `traefik.your-domain.com`.
