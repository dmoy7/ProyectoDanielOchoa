# Proyecto: Análisis de Series de TV en Enero 2024

## Descripción

Este proyecto tiene como objetivo la extracción, limpieza, análisis y almacenamiento, de datos de series de TV emitidas en enero de 2024, 
utilizando la API de TVMaze. Se generan reportes de profiling, se transforman los datos en un modelo estructurado y se almacenan en una 
base de datos SQLite para realizar operaciones de agregación.

## Estructura del Proyecto

├── README.md
├── src/
│   ├── carga.py  # Carga datos en SQLite y realiza consultas
├── json/
│   ├── tvmaze_2024-01-01.json  # Datos crudos extraídos de la API
├── profiling/
│   ├── tvmaze_profiling_before.html  # Profiling antes de limpieza
│   ├── tvmaze_profiling_after.html  # Profiling después de limpieza
│   ├── AnalisisPerfilamento.pdf  # Archivo con análisis de perfilamiento
├── data/
│   ├── tvmaze_limpiado.parquet  # Datos limpios en formato Parquet
├── db/
│   ├── tv_shows.db  # Base de datos SQLite con datos transformados
├── model/
│   ├── Modelo.pdf  # Modelo relacional de la base de datos

## Requisitos

- Python 3.x

- Librerías: pandas, requests, ydata-profiling, sqlite3, pyarrow

## Ejecución del Proyecto

1. Ejecución de extracción y transformación: Clase TVMazeDataCollector del notebook EntregableDanielOchoa.ipynb, con el fin de obtener el archivo parquet con los datos limpios (tvmaze_limpiado).
2. Ejecución carga a base de datos: Clase TVShowDatabase del notebook EntregableDanielOchoa.ipynb, con el fin de cargar la información en una base de datos de SQLite (tv_shows.db).

## Análisis y Resultados

- Runtime promedio de los shows emitidos en enero de 2024.
- Conteo de shows por género.
- Dominios únicos de los sitios oficiales de los shows.

## Contacto

Autor: Daniel Ochoa

Repositorio: [GitHub](https://github.com/dmoy7)


