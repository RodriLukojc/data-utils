# data-utils — Entorno reproducible para análisis y pipelines de datos

[![CI](https://github.com/RodriLukojc/data-utils/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/RodriLukojc/data-utils/actions/workflows/ci.yml)
[![Release](https://github.com/RodriLukojc/data-utils/actions/workflows/release.yml/badge.svg?branch=main)](https://github.com/RodriLukojc/data-utils/actions/workflows/release.yml)
[![Docker Hub](https://img.shields.io/badge/DockerHub-data--utils-blue?logo=docker)](https://hub.docker.com/r/rodrigolukojc/data-utils)

---

## 📌 Descripción

data-utils es una imagen Docker diseñada como **entorno base para análisis de datos, automatización de pipelines y experimentación reproducible**.

Incluye herramientas esenciales para:

- Limpieza y transformación de datos  
- Automatización de procesos analíticos  
- Ejecución de scripts Python orientados a ETL  
- Reproducibilidad de entornos para Data Analytics y Data Engineering  
- Integración con CI/CD para flujos de datos versionados  

Este proyecto forma parte de mi portafolio profesional como **Analista de Datos / Ingeniero de Datos**, demostrando buenas prácticas de ingeniería aplicadas al mundo del análisis.

---

## Características principales

- Imagen ligera basada en Python 3.10  
- Librerías esenciales para análisis de datos (Pandas, NumPy, etc.)  
- Scripts utilitarios para pipelines ETL  
- CI/CD completo con GitHub Actions  
- Versionado semántico automático (v1.0.0, v1.1.0, etc.)  
- Publicación automática en Docker Hub  
- Entorno reproducible para análisis, pruebas y automatización  

---

## Cómo usar la imagen

### Obtener la última versión estable

docker pull rodrigolukojc/data-utils:latest
Obtener una versión específica
bash
docker pull rodrigolukojc/data-utils:v1.0.0
Ejecutar un script de análisis
bash
docker run -it --rm \
  -v $(pwd)/data:/app/data \
  rodrigolukojc/data-utils:latest \
  python src/etl_example.py

Estructura del proyecto

Código

data-utils/
├── Dockerfile
├── requirements.txt
├── src/
│   ├── etl_example.py        # Ejemplo de pipeline ETL
│   └── utils/                # Funciones auxiliares
├── examples/
│   └── notebook.ipynb        # Notebook de análisis (opcional)
├── .github/
│   └── workflows/
│       ├── ci.yml
│       └── release.yml
└── README.md

Versionado
Este proyecto utiliza versionado semántico para garantizar reproducibilidad en pipelines de datos.

Crear una nueva versión:

git tag v1.1.0
git push origin v1.1.0
Esto dispara automáticamente la publicación en Docker Hub.

CI/CD

CI — Integración Continua
Instala dependencias

Ejecuta tests

Construye la imagen

Publica latest

CD — Entrega Continua
Se ejecuta al crear un tag

Publica:

latest

vX.Y.Z

Ejemplo de pipeline ETL incluido
El archivo src/etl_example.py muestra un flujo simple:

Lectura de CSV

Limpieza de datos

Transformaciones

Generación de KPIs

Exportación de resultados

Este ejemplo demuestra cómo usar la imagen como entorno analítico reproducible.

Roadmap

[ ] Añadir conectores a APIs y bases SQL

[ ] Incluir notebooks de análisis reales

[ ] Integrar Airflow o Prefect para orquestación

[ ] Añadir validación de datos con Great Expectations

[ ] Publicar dataset de ejemplo para reproducir pipelines

[ ] Crear dashboard Power BI conectado al pipeline

Autor
Rodrigo Lukojc  
Analista de Datos · Ingeniería de Datos · Automatización de Procesos
Buenos Aires, Argentina

🔗 LinkedIn: https://www.linkedin.com/in/rodrigolukojc (linkedin.com in Bing)  
🐳 Docker Hub: https://hub.docker.com/u/rodrigolukojc (hub.docker.com in Bing)  
📂 GitHub: https://github.com/rodrigolukojc (github.com in Bing)

Licencia
MIT License.
