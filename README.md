# Traefik Docker Setup

Este repositorio contiene una configuración de Traefik para implementar como proxy reverso y gestor de certificados SSL.


## Instalación rápida

1. Clona este repositorio:

2. Copia el archivo de ejemplo y crea tu configuración:
   ```bash
   cp .env.example .env
   ```

3. Crea la red externa de Docker que usará Traefik:
   ```bash
   docker network create traefik
   ```

5. Inicia Traefik con Docker Compose:
   ```bash
   docker-compose up -d
   ```

## Acceso al panel de administración

Una vez que Traefik esté en funcionamiento, puedes acceder al panel de administración en:

```
https://monitor.tudominio.com
```

Utiliza las credenciales que configuraste en la variable `TRAEFIK_LOGIN` del archivo `.env`.
