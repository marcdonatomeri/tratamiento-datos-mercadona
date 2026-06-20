# 🛒 Proyecto Tratamiento de Datos — Análisis de Tickets de Mercadona

Proyecto de la asignatura **Tratamiento de Datos** (1º de carrera) que extrae, limpia y analiza la información contenida en **tickets de compra de Mercadona** en formato PDF, usando **R**.

## 🎯 Objetivo

Convertir cientos de tickets PDF en un conjunto de datos estructurado (productos, precios, fechas, importes, etc.) para realizar análisis exploratorio sobre los hábitos y patrones de compra.

## ⚙️ Cómo funciona

El procesamiento parte de la función `procesar_ticket()`, que para cada PDF:

1. Extrae el texto con la librería **`pdftools`**.
2. Identifica los datos de cabecera (ubicación, código postal, fecha, hora, importe total, IVA…).
3. Parsea la lista de productos (descripción, precio unitario, peso, importe).
4. Construye un *data frame* unificado con todos los tickets para su análisis.

## 📁 Estructura

```
.
├── Proyecto_TD_2025.Rmd        # Informe principal: procesado y análisis
├── Proyecto_TD_2025.html/.pdf  # Informe renderizado
├── Pruebas Marc Donato.Rmd     # Pruebas y desarrollo
├── productos_global.csv        # Productos extraídos de todos los tickets
├── tickets_global.csv          # Cabeceras de todos los tickets
├── ProyectoTD2025.Rproj        # Proyecto de RStudio
├── data/                       # Tickets de Mercadona en PDF (datos de entrada)
└── Memoria Proyecto TD/        # Memoria del proyecto (RMarkdown + LaTeX)
```

## 🚀 Uso

Requisitos: **R** (con RStudio recomendado) y los siguientes paquetes:

```r
install.packages(c("pdftools", "stringr", "dplyr", "lubridate", "ggplot2"))
```

Abre `ProyectoTD2025.Rproj` en RStudio y renderiza `Proyecto_TD_2025.Rmd` (botón *Knit*) para reproducir el procesado y los análisis.

## 🛠️ Tecnologías

- **R** — pdftools, stringr, dplyr, lubridate, ggplot2
- **RMarkdown** + **LaTeX** para la memoria e informes

## 👥 Autores

José Ignacio Calatayud Cuenca · Marc Donato Merí · Manuel Giner Flores · Marc Navarro Montava · Eduardo Oltra Ramos · Isaac Ruiz Quitero
