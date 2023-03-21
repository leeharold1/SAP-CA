# main branch

```
docker network create CA2Lee
docker run --name db -e MYSQL_ROOT_PASSWORD=my-secret-password -d mysql:latest
docker run --name phpmyadmin -d -p 8080:80 --network CA2Lee phpmyadmin/phpmyadmin
```