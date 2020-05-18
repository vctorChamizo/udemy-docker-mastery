# Docker | Bindmount assignment

## Persistent Data: Data Volumes
```
docker pull mysql

docker container run -d --name mysql -e MYSQL_ALLOW_EMPTY_PASSWORD=True mysql

docker container ls

docker container inspect mysql

docker volume ls

docker container stop mysql

docker container ls

docker container ls -a

docker volume create --help
```

---

## Persistent Data: Bind Mounting

```
docker container run -d --name nginx -p 80:80 -v $(pwd):/usr/share/nginx/html nginx

docker container exec -it nginx bash
```

---

## Assignment Answers: Edit Code Running In Containers With Bind Mounts

```
docker run -p 80:4000 -v $(pwd):/site bretfisher/jekyll-serve
```
