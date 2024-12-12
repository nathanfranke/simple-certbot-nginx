### ❤️ Consider using [jonasal/nginx-certbot](https://github.com/JonasAlfredsson/docker-nginx-certbot) for the HTTP-01 challenge. [See here](https://letsencrypt.org/docs/challenge-types/) for the benefits and drawbacks of each challenge type.

# docker-certbot-nginx-cloudflare

Usage:
- Forward ports `80` and `443`, and route a subdomain to your server.
- Create `cloudflare.ini` with [your API token](https://certbot-dns-cloudflare.readthedocs.io/en/stable/#credentials). Use `chmod 600 cloudflare.ini` to fix its permissions.
- Change `example.com` in `docker-compose.yml` and `conf.d/default.conf`. Also change the email and subdomain, if you want.
- Run `docker-compose up` and wait for nginx to start. If it is successful, you can visit your subdomain.
