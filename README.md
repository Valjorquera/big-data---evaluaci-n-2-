theme: jekyll-theme-cayman
# Evaluaci-n-big-data
Repositorio para la evaluación 2 big data
# Evaluación Parcial 2 - Big Data
# Evaluación Parcial 2 - Big Data

**Nombres Antonella de los Ángeles Ugalde Bruna  Valentina Jorquera
**Asignatura:** AVY1101 - Big Data  
**Evaluación:** Evaluación Parcial N°2  
**Modalidad:** Batch – Proyecto Big Data  
**Repositorio:** Sitio de Proyecto GitHub  
**Fecha de entrega:** [Agrega la fecha aquí]

---

## 📌 Índice

1. [Introducción](#1-introducción)  
2. [Conexión y obtención de datos](#2-conexión-y-obtención-de-datos)  
3. [DataLake y almacenamiento](#3-datalake-y-almacenamiento)  
4. [Limpieza y transformación](#4-limpieza-y-transformación)  
5. [Validación, errores y control de duplicados](#5-validación-errores-y-control-de-duplicados)  
6. [Visualización y análisis (Dashboard)](#6-visualización-y-análisis-dashboard)  
7. [Conclusiones](#7-conclusiones)  
8. [Anexos](#8-anexos)

---

## 1. Introducción

El presente proyecto corresponde a la Evaluación Parcial N°2 de la asignatura de Big Data, y tiene como objetivo aplicar los conocimientos sobre procesos Batch para la ingesta, transformación, almacenamiento y análisis de grandes volúmenes de datos en un entorno de Big Data.

Se aborda una carga histórica de datos desde diversas fuentes, considerando criterios de validación, control de errores y visualización de insights relevantes mediante dashboards interactivos. Este proceso permitirá responder preguntas clave del negocio y simular un flujo completo de procesamiento de datos en la nube.

---

## 2. Conexión y obtención de datos

Para este proyecto se trabajó con datos obtenidos desde [nombre fuente, por ejemplo: archivos CSV públicos / Kaggle / bases simuladas].

Los archivos fueron descargados desde:  
- [URL del dataset o fuente de datos]  
- En formato: `.csv`, `.json`, [otro]  

La obtención se automatizó mediante scripts en Python utilizando bibliotecas como `pandas`, `requests` o conectores específicos, y fueron guardados inicialmente en el entorno local / GCS.

---

## 3. DataLake y almacenamiento

Se utilizó un enfoque de almacenamiento en un DataLake basado en [elige uno: Google Cloud Storage / BigQuery / Amazon S3].

Estructura del almacenamiento:

DataLake/
│
├── raw/ # Datos originales
├── processed/ # Datos limpios y transformados
└── analytics/ # Tablas para análisis y visualización

Los datos fueron cargados en el DataLake usando comandos SQL o scripts automatizados con `bq`, `gsutil` o herramientas de ETL como [indica cuál usaste].

---

## 4. Limpieza y transformación

Los datos presentaban diversos problemas que fueron abordados en esta etapa:

- Eliminación de filas con valores nulos
- Conversión de tipos de datos (fechas, números)
- Normalización de nombres y formatos
- Eliminación de duplicados
- Creación de nuevas columnas para análisis
- Agregación por categorías o fechas

La transformación se implementó en Python con `pandas` y luego se cargaron en una tabla final para análisis en BigQuery.

---

## 5. Validación, errores y control de duplicados

Se incorporaron controles para asegurar la calidad y estabilidad del flujo:

- Validación de estructura del archivo (columnas obligatorias)
- Control de duplicados: verificación con hashes o claves únicas
- Control de ejecución: registro de procesos realizados (log)
- Manejo de errores: try/except y alertas en consola/logs
- Reprocesamiento histórico: opción de volver a ejecutar por fecha

---

## 6. Visualización y análisis (Dashboard)

Se construyeron 4 gráficos representativos utilizando [Python / Power BI / Tableau]:

1. 📊 Distribución por categoría  
2. 📈 Evolución temporal  
3. 🧭 Comparación entre grupos  
4. 📌 Análisis predictivo básico (opcional)

![grafico1](visualizations/grafico1.png)  
![grafico2](visualizations/grafico2.png)

Los gráficos permiten extraer insights clave que pueden apoyar la toma de decisiones del área de negocio.

---

## 7. Conclusiones

El desarrollo de este proyecto permitió simular un flujo completo de procesamiento Batch en un entorno Big Data, comprendiendo desde la ingesta hasta la entrega de visualizaciones analíticas. Se lograron identificar errores comunes, automatizar procesos y estructurar un flujo robusto, útil para la operación de datos a gran escala.

Además, se reforzaron habilidades en limpieza, transformación y uso de herramientas en la nube como GCP, junto con la capacidad de comunicar resultados visualmente.

---

## 8. Anexos

- Script de descarga de datos: `scripts/descarga_datos.py`
- Script de limpieza: `scripts/limpieza.py`
- SQL para carga en BigQuery: `scripts/carga_bq.sql`
- Gráficos: carpeta `/visualizations/`
- Diagrama del flujo de proceso: [opcional: puedes subir una imagen]

---
