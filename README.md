# Trabalho 1 Sistemas Operacionais

Ambiente virtualizado utilizando Docker utilizando Nginx.

## Execução

Primeiramente, executando com o docker-compose

```bash
docker-compose up -d
# or
sudo docker-compose up -d
```

Verificar em localhost:80/

Para desativar a execução:

```bash
docker-compose down
# or
sudo docker-compose down
```

Em seguida, temos a utilização do build do DockerFile

```bash
sudo docker build -t docker_nginx . 

sudo docker run --name docker_nginx_container -p 27016:80 docker_nginx
```

Verificar em 0.0.0.0:27016/