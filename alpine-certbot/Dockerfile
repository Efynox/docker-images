FROM alpine:3.4

RUN apk add --no-cache certbot

VOLUME /etc/letsencrypt
VOLUME /var/lib/letsencrypt

EXPOSE 80 443

ENTRYPOINT certbot