# Monitoreo de la Crisis de Desapariciones en México (2024): Análisis Espacial y Demográfico


Este proyecto presenta una visualización de datos del Registro Nacional de Personas Desaparecidas y No Localizadas (RNPDNO) correspondiente al año 2024 con Tableu.


## Visualización Interactiva de los Datos

El tablero completo está publicado en Tableau Public y permite la interacción dinámica con los mapas:

[![Ver en Tableau Public](https://img.shields.io/badge/Ver_Dashboard-Tableau_Public-E95420?style=for-the-badge&logo=tableau)](https://public.tableau.com/app/profile/c.sar.romero6323/viz/MonitoreodelaCrisisdeDesaparicionesenMxicoAnlisisEspacialyDemogrfico2024/Storytelling?publish=yes)

> **Haz clic en el botón de arriba para explorar la historia completa.**

---

## Hallazgo: La Opacidad del 67% en el Registro

El análisis de 103,417 registros procesados revela una falla sistémica en la captura de datos gubernamentales:

* **Total de Registros:** 103,417
* **Sin Ubicación (No Especificado):** 69,704 (67.4%)
* **Ubicación Confirmada:** 33,713 (32.6%)

> **Nota Metodológica:** Los mapas presentados representan únicamente la "geografía visible" (el 32.6% de los casos). Las tasas de violencia por cada 100,000 habitantes constituyen un umbral mínimo confirmado, ya que la magnitud real es significativamente mayor pero territorialmente indeterminada.

## Metodología e Ingeniería de Datos

Este proyecto es la fase de análisis visual de un flujo de trabajo más complejo. La obtención de los datos se realizó mediante la técnica de web scraping con Rust y el procesamiento de datos con RStudio.

### 1. Extracción
La descarga masiva de los registros JSON del RNPDNO se realizó utilizando Rust para manejar el volumen de datos.

* **Código Fuente del Scraper:** Puedes consultar el repositorio aquí:
  [RomeroStats/Web_Scraping_Rust_y_RStudio](https://github.com/RomeroStats/Web_Scraping_Rust_y_RStudio)

### 2. Procesamiento y Limpieza (RStudio)
Se utilizó RStudio para la integración y limpieza de los archivos.

### 3. Visualización (Tableau)
Diseño de Storytelling para contrastar la magnitud absoluta vs. relativa (Tasas por 100,000 habitantes) y análisis demográfico.

## Autor

**Mtro. José César Romero Galván**
