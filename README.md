docker-https
============

Simple docker compose file for nginx with https only.

Usage
-----
Put certificate under `./certs/ota.crt` and private key under `./certs/ota.key`.
Put the files to serve under `./htroot`.

To create a self-signed certificate, run:
```
openssl req -x509 -nodes -days 3650 -newkey rsa:2048 -keyout ota.key -out ota.crt
```
When asked for "common name", enter your domain name.
