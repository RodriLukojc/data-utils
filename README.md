# utils-infra  
Herramientas de infraestructura, automatización y soporte técnico empaquetadas en una imagen Docker ligera y reproducible.

[![CI](https://github.com/RodriLukojc/utils-infra/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/RodriLukojc/utils-infra/actions/workflows/ci.yml)
[![Release](https://github.com/RodriLukojc/utils-infra/actions/workflows/release.yml/badge.svg?branch=main)](https://github.com/RodriLukojc/utils-infra/actions/workflows/release.yml)
[![Docker Hub](https://img.shields.io/badge/DockerHub-utils--infra-blue?logo=docker)](https://hub.docker.com/r/rodrigolukojc/utils-infra)

---

## Descripción

"utils-infra" es una imagen Docker diseñada para centralizar herramientas de infraestructura, automatización y soporte técnico en un entorno portátil y reproducible.

Este proyecto forma parte de mi portafolio profesional orientado a:

- **Data Analytics**
- **Infraestructura ligera**
- **Automatización de procesos**
- **Buenas prácticas de CI/CD**

La imagen se publica automáticamente en Docker Hub utilizando **GitHub Actions**, con soporte para:

- latest  
- Versionado semántico ("v1.0.0", "v1.1.0", etc.)

---

## Características principales

- Imagen ligera basada en Linux
- Herramientas de automatización y soporte incluidas
- Pipeline CI/CD completo con:
  - Build automático
  - Tests (placeholder)
  - Publicación en Docker Hub
  - Versionado semántico automático
- Reproducible y portable
- Ideal para tareas de:
  - Infraestructura
  - DataOps
  - Scripts de mantenimiento
  - Procesos ETL simples

---

## Cómo usar la imagen

### Obtener la última versión estable

docker pull rodrigolukojc/utils-infra:latest

Obtener una versión específica

docker pull rodrigolukojc/utils-infra:v1.0.0

Ejecutar la imagen

docker run -it --rm rodrigolukojc/utils-infra:latest bash

Versionado
Este proyecto utiliza versionado semántico:

MAJOR: cambios incompatibles

MINOR: nuevas funcionalidades

PATCH: correcciones

Las versiones se generan automáticamente al crear un tag:

git tag v1.0.0
git push origin v1.0.0

CI/CD

El repositorio incluye dos workflows:

1. CI (Integración Continua)

Instala dependencias

Ejecuta tests

Construye la imagen local

Publica latest en Docker Hub

2. Release (Entrega Continua)

Se ejecuta solo cuando se crea un tag v*.*.*

Publica:

latest

vX.Y.Z

Estructura del proyecto
Código
utils-infra/
├── Dockerfile
├── requirements.txt
├── src/
│   └── ...
├── .github/
│   └── workflows/
│       ├── ci.yml
│       └── release.yml
└── README.md

Autor
Rodrigo Lukojc  
Data Analytics
Buenos Aires, Argentina

🔗 LinkedIn: https://www.linkedin.com/in/rodrigolukojc (linkedin.com in Bing)  
🐳 Docker Hub: https://hub.docker.com/u/rodrigolukojc (hub.docker.com in Bing)  
📂 GitHub: https://github.com/rodrigolukojc (github.com in Bing)

⭐ Contribuciones
Este proyecto forma parte de mi portafolio profesional.
Las sugerencias, issues y mejoras son bienvenidas.

📜 Licencia
MIT License.
