# [MYSQL] (https://hub.docker.com/_/mysql)


```bash
docker run \
    --name <이미지 이름> \
    -p <로컬 포트>:3306 \
    -e MYSQL_ROOT_PASSWORD=<패스워드> \
     -v <로컬 마운트 경로>:/var/lib/mysql \ 
     -d mysql:9.5.0
```

```bash
docker run \
    --name mydata \
    -p 3306:3306 \
    -e MYSQL_ROOT_PASSWORD=docker123 \
    -v C:/Users/USER/Documents/dockerdata/mysqldata:/var/lib/mysql \
    -d mysql:9.5.0
```

# Build
```bash
docker build -t \
    ghcr.io/<Namespace>/<이미지 이름>:<이미지 태그>-<버전>
```

```bash
docker build -t ghcr.io/parkjinwon1025/hello:mysql-9.5.0
```

# Publishing

# Installing