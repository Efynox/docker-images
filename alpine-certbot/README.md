# efynox/alpine-certbot
## Usage
### Create a new certificat
```
docker run --rm \
  -p 443:443 -p 80:80 \
  -v /root/cert:/etc/letsencrypt \
  efynox/alpine-certbot certonly \
    --standalone \
    --text \
    --email email@example.com \
    --agree-tos \
    --standalone-supported-challenges http-01 \
    --domains example.com \
    --domains www.example.com
```