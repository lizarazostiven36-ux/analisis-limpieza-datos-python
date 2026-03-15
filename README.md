# Movilidad Urbana y Economía en LATAM – Python

## Descripción del Proyecto

Como analista de datos, el objetivo de este proyecto es evaluar cómo la movilidad urbana se relaciona con la productividad económica en las principales ciudades latinoamericanas.

Para ello se trabajó con datos reales de **TomTom Traffic Index** y **OECD Cities**, que fueron limpiados, combinados y analizados para identificar en qué ciudades conviene invertir en infraestructura de transporte.

Este análisis fue desarrollado como parte del programa de **Analista de Datos de TripleTen**.

---

## Objetivo

Identificar la relación entre el nivel de congestión vehicular y el PIB per cápita en ciudades latinoamericanas, para apoyar decisiones de inversión en infraestructura de transporte.

---

## Dataset

| Archivo | Descripción |
|---|---|
| `tomtom_traffic.csv` | Datos de tráfico y congestión vehicular por ciudad (TomTom Traffic Index) |
| `oecd_city_economy.csv` | Datos económicos por ciudad: PIB per cápita, población (OECD Cities) |

### Columnas principales

| Columna | Descripción |
|---|---|
| `Country` | País de la ciudad |
| `City` | Nombre de la ciudad |
| `JamsDelay` | Retraso promedio en minutos por congestión |
| `JamsCount` | Número de embotellamientos registrados |
| `TrafficIndexLive` | Índice de tráfico en tiempo real |
| `TravelTimeLivePer10KmsMin` | Tiempo de viaje por cada 10 km en minutos |

---

## Proceso de Análisis

### 1. Carga y exploración de datos
- Importación de librerías: `pandas`, `numpy`, `seaborn`, `matplotlib`
- Carga de los archivos CSV en DataFrames
- Vista previa de los primeros registros y estructura de columnas

### 2. Identificación de valores faltantes
- Detección de nulos con `.isnull().sum()`
- Análisis del porcentaje de datos faltantes por columna

### 3. Eliminación de duplicados
- Verificación y eliminación de registros duplicados

### 4. Corrección de formatos incorrectos
- Estandarización de tipos de datos
- Conversión de columnas de fecha y valores numéricos

### 5. Análisis exploratorio de datos (EDA)
- Estadísticas descriptivas por ciudad y país
- Identificación de ciudades con mayor congestión
- Comparación entre niveles de tráfico y economía

### 6. Visualización de patrones y tendencias
- Gráficas de barras por nivel de congestión
- Análisis de correlación entre congestión y PIB per cápita
- Identificación de outliers y ciudades atípicas

---

## Principales Hallazgos

- 🏙️ **Ciudad de México** presentó el mayor nivel de congestión con **2,833 unidades** en `jams_delay`.
- 📊 Se identificó una relación entre el nivel de congestión vehicular y el PIB per cápita de las ciudades.
- 🌎 Las ciudades latinoamericanas con mayor congestión tienden a tener mayor actividad económica, pero también mayores costos de movilidad.
- 💡 Las ciudades con mejor infraestructura de transporte mostraron tiempos de viaje significativamente menores por cada 10 km.

---

## Estructura del Proyecto

```
analisis-limpieza-datos-python/
│
├── README.md
└── 55_ladb_mobility_economy_project_student.ipynb
```

---

## Herramientas Utilizadas

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Autor

**Stiven Lizarazo**  
Analista de Datos Junior  
Proyecto desarrollado como parte del programa de Análisis de Datos de TripleTen.
