# Nextcloud Docker Deployment

Proyecto para desplegar Nextcloud usando Docker Compose.

## Descripción
Este repositorio contiene la configuración básica para desplegar Nextcloud en contenedores Docker usando `docker-compose`.

## Requisitos
- Docker
- Docker Compose

## Uso
1. Clona el repositorio:

```bash
git clone <repo-url>
cd nextcloud-docker
```

2. Inicia los servicios:

```bash
docker-compose up -d
```

3. Para ver logs:

```bash
docker-compose logs -f
```

4. Para detener y eliminar contenedores:

```bash
docker-compose down
```

## Persistencia
Asegúrate de revisar los volúmenes en `docker-compose.yml` para ofrecer persistencia de datos y configuración.

## Contribuir
Sugerencias y pull requests son bienvenidos.

## Licencia
Revisa la licencia del proyecto (si aplica).