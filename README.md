Comando para construir la imagen desde dockerfile
```sh
docker build -t demo-httpd:L14 .
```


Ejecutar la imagen construida:

```sh
docker run -p 3000:80 demo-httpd:L14
```

Usar el docker-compose

Para utilizar el docker-compose se utiliza un archivo denominado
`docker-compose.yml`

Para dar de alta los servicios definidos en el docker-compose se debe ejecutar el siguiente comando

```sh
docker-compose up -d
```

Para detener los servicios se debe ejecutar lo siguiente:
```sh
docker-compose stop
```

Para volver a iniciar los servicios se debe ejecutar lo siguiente:
```sh
docker-compose start
```

Para desinstalar los servicios del contenedor se debe ejecutar lo siguiente:
```sh
docker-compose down
```

Si se necesita reconstruir la imagen de los servicios con docker-compose, se utiliza el siguiente comando:
```sh
docker-compose up -d --build
```
------------ADICIONAL
COMO SABER QUE CONTENEDORES SE ESTAN UTILIZANDO/EJECUTANDO
Consultar el estado de los contenedores:
```sh
docker ps
```


```sh
docker stop carpeta-mysql-1
```

```sh
docker start 68b38790a1bf
```