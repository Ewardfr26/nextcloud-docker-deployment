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

## Seguridad
- **No subas secretos:** No incluyas ` .env ` ni archivos con contraseñas en el repositorio.
- **Usa ` .env.example `:** Copia ` .env.example ` a ` .env ` y rellena los valores en tu máquina local.
- **Generar contraseñas seguras:** Usa generadores de contraseñas, por ejemplo:

```bash
# Genera 32 caracteres con OpenSSL
openssl rand -base64 24

# O con pwgen si está instalado
pwgen 32 1
```

- **Alternativas seguras:** Considera usar Docker secrets, un gestor de secretos (HashiCorp Vault, AWS Secrets Manager) o variables de entorno proporcionadas por tu orquestador.
- **Permisos y backups:** Protege los volúmenes que contienen `nextcloud/data` y las copias de seguridad; realiza backups regulares y restringe permisos de acceso.

Si deseas, puedo añadir instrucciones para integrar Docker secrets o un ejemplo de script para generar `.env` desde variables de entorno.