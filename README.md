# Streaming Platforms BI & Data Model 🎬

🌍 *[Read in English](#-english-version) | [Leer en Español](#-versión-en-español)*

---

## 🇬🇧 English Version

### 📌 Project Overview
This project consists of the design and implementation of a relational data model and Business Intelligence dashboard for analyzing movies distributed across streaming platforms (Netflix and Disney+).

The main objective is to structure the data into an analytics-optimized schema that enables business insights related to:
* Movie popularity and ratings
* Director performance and ROI
* Geographic distribution
* Platform comparison and catalog overlap
* Yearly production trends and average runtime

*(The dataset contains 4,112 movies updated until early 2020).*

### 🧱 Data Architecture & Modeling
The model follows a strict **Star Schema**, ensuring optimized query performance and relational integrity through Primary Keys (PK) and Foreign Keys (FK):
* **Fact Table:** `General` (central movie attributes and quantitative metrics).
* **Dimension Tables:** `Platforms`, `Directors`, `Genres`, `Countries`, `Languages`, `Age Classification`, and a dedicated `Calendar` table for time-series analysis.

### 🔄 Data Transformations (ETL)
* Normalization of ID fields across raw datasets.
* Rotten Tomatoes scores adjusted for standardized analytical comparison.
* DAX measures implemented for dynamic KPI calculation.

### 📊 Implemented KPIs
* Total Movies & Movies per Platform
* Distinct Directors & Genres
* Average Runtime & IMDb Score

### 🎯 Business Objective
The developed dashboard enables tactical-level interactive analysis, supporting decision-making processes in the entertainment industry. It allows stakeholders to explore catalog patterns, platform comparisons, and content trends.

### 🛠 Tools Used
* **Business Intelligence:** Power BI
* **Data Engineering:** Relational Data Modeling, Data Normalization
* **Analytics:** DAX (Data Analysis Expressions)

### 🚀 Phase 2: Cloud Architecture Roadmap
* SQL-based schema implementation (Relational Database mapping).
* Cloud Data Warehouse migration.
* Integration of `dbt` (data build tool) for the transformation layer.
* Automated data pipeline execution.

---

## 🇪🇸 Versión en Español

### 📌 Descripción del Proyecto
Este proyecto consiste en el diseño e implementación de un modelo de datos relacional y un dashboard de Business Intelligence orientado al análisis de contenido distribuido en plataformas de streaming (Netflix y Disney+).

El objetivo principal es estructurar la información en un esquema optimizado que permita generar *insights* de negocio relacionados con:
* Popularidad y valoraciones del contenido
* Rendimiento de directores 
* Distribución geográfica
* Comparación de catálogos entre plataformas
* Tendencias de producción por año y duración promedio

*(El dataset incluye 4.112 películas con información actualizada hasta principios de 2020).*

### 🧱 Arquitectura y Modelado de Datos
El modelo sigue una estructura de **Esquema de Estrella (Star Schema)** pura, garantizando rendimiento analítico e integridad referencial mediante Claves Primarias (PK) y Foráneas (FK):
* **Tabla de Hechos (Fact Table):** `General` (información central y métricas cuantitativas).
* **Tablas de Dimensión:** `Plataformas`, `Directores`, `Géneros`, `Países`, `Idiomas`, `Clasificación por Edad`, y una tabla `Calendario` para inteligencia de tiempo.

### 🔄 Transformaciones Realizadas (ETL)
* Normalización de campos ID desde las fuentes crudas.
* Ajuste de la variable de Rotten Tomatoes para estandarización analítica.
* Implementación de medidas complejas en DAX para el cálculo dinámico de KPIs.

### 📊 KPIs Implementados
* Cantidad total de películas y distribución por plataforma
* Cantidad de directores y géneros únicos
* Duración promedio y promedio de puntuación IMDb

### 🎯 Objetivo de Negocio
El dashboard desarrollado permite un análisis interactivo a nivel táctico, facilitando la toma de decisiones en el sector del entretenimiento. Permite a los *stakeholders* identificar patrones de catálogo, comparar plataformas y detectar tendencias clave.

### 🛠 Herramientas Utilizadas
* **Business Intelligence:** Power BI
* **Ingeniería de Datos:** Modelado Relacional, Normalización de Datos
* **Analítica:** DAX (Data Analysis Expressions)

### 🚀 Fase 2: Roadmap de Arquitectura Cloud
* Implementación del modelo físico en SQL.
* Migración hacia un Data Warehouse en la nube.
* Capa de transformación escalable utilizando `dbt`.
* Automatización del *pipeline* de ingesta de datos.
