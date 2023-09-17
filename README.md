# Docker One-Liners

A list of handy Docker one-liners.

## Interactive Ubuntu Image

```
docker run -it ubuntu
```

## Quick Nginx

```
docker run -p 8080:80 nginx
```

## Setup SSL on Ubuntu/Nginx
Site must be configured on registry already and Nginx must be configured to run the site.

```
snap install core
snap refresh core
snap install --classic certbot
ln -s /snap/bin/certbot /usr/bin/certbot
certbot --nginx
# Answer questions
```

