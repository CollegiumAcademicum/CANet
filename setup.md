- Pull this repo onto the server

```bash
bash install.sh
docker-compose up -d
docker cp proxy.conf swag:/config/nginx/proxy-confs/proxy.conf
```

go to wiki.ca-hd.net/install.php