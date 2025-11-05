# Frontend - Sistema de Comentarios

HTML simple con JavaScript que consume la API de backend.

## Build Local

```bash
docker build -t comments-frontend:local .
docker run -p 8080:80 comments-frontend:local
```

## CI/CD

El pipeline de GitHub Actions:
1. Construye la imagen Docker
2. La sube a Docker Hub con tag del build number
3. Usar ese número en helm-chart/values.yaml
