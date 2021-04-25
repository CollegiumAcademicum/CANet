- Pull this repo onto the server

```bash
bash install.sh
docker kill $(docker ps -q)
docker rm $(docker ps -a -q)
docker-compose up -d
docker network inspect canet_default 
docker ps
docker cp site-confs.conf swag:/config/nginx/site-confs/default
docker restart swag
```

go to wiki.ca-hd.net/install.php