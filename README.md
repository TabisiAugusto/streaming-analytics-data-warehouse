# Streaming Analytics Data Warehouse. Modelado de datos y análisis de plataformas de streaming
🇪🇸 Versión en Español
📌 Descripción del Proyecto

Este proyecto consiste en el diseño e implementación de un modelo de datos relacional orientado al análisis de películas distribuidas en plataformas de streaming (Netflix y Disney+).

El objetivo principal es estructurar la información en un esquema optimizado para análisis, permitiendo generar insights de negocio relacionados con:

Popularidad y valoraciones de películas

Rendimiento de directores

Distribución geográfica

Comparación entre plataformas

Tendencias por año

Duración promedio de contenido

El dataset incluye 4.112 películas con información actualizada hasta principios de 2020.

🧱 Arquitectura de Datos

El modelo sigue una estructura inspirada en un esquema estrella, compuesta por:

Tabla principal (tipo fact):

General (información central de cada película)

Tablas dimensión:

Plataformas

Directores

Géneros

Países

Idiomas

Clasificación por edad

Calendario

Se definieron claves primarias (PK) y claves foráneas (FK) para asegurar integridad relacional.

🔄 Transformaciones Realizadas

Normalización de campos ID.

Ajuste de la variable Rotten Tomatoes para facilitar comparación analítica.

Creación de tabla calendario para análisis temporal.

Implementación de medidas calculadas (DAX) para indicadores clave.

📊 Indicadores Implementados

Cantidad total de películas

Películas por plataforma

Cantidad de directores únicos

Cantidad de géneros

Duración promedio

Promedio de puntuación IMDb

🎯 Objetivo de Negocio

El dashboard desarrollado permite análisis interactivo orientado a nivel táctico, facilitando la exploración de datos para toma de decisiones en el sector streaming / entretenimiento.

Permite identificar patrones, comparaciones y tendencias relevantes.

🛠 Herramientas Utilizadas

Power BI

Modelado relacional

DAX

Normalización de datos

🚀 Próximas Mejoras

Implementación del modelo en SQL

Migración a Data Warehouse en la nube

Capa de transformación con dbt

Automatización del pipeline de datos

🇺🇸 English Version
📌 Project Overview

This project consists of the design and implementation of a relational data model for analyzing movies distributed across streaming platforms (Netflix and Disney+).

The main objective is to structure the data into an analytics-optimized schema that enables business insights related to:

Movie popularity and ratings

Director performance

Geographic distribution

Platform comparison

Yearly trends

Average runtime

The dataset contains 4,112 movies updated until early 2020.

🧱 Data Architecture

The model follows a star-schema inspired structure, composed of:

Main table (fact-like):

General (central movie attributes)

Dimension tables:

Platforms

Directors

Genres

Countries

Languages

Age classification

Calendar table

Primary and foreign keys were defined to ensure relational integrity.

🔄 Transformations Performed

ID field normalization.

Rotten Tomatoes score adjusted for analytical comparison.

Calendar table creation for time-based analysis.

DAX measures implemented for KPI calculation.

📊 Implemented Metrics

Total Movies

Movies per Platform

Distinct Directors

Distinct Genres

Average Runtime

Average IMDb Score

🎯 Business Objective

The dashboard enables tactical-level interactive analysis, supporting decision-making processes in the streaming and entertainment industry.

It allows users to explore patterns, comparisons and relevant trends.

🛠 Tools Used

Power BI

Relational Data Modeling

DAX

Data normalization techniques

🚀 Future Improvements

SQL-based schema implementation

Cloud Data Warehouse migration

dbt transformation layer

Automated data pipeline integration
