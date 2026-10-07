# 🚀 DaniMarket - ECommerce Big Data Analytics Project

---

# 📌 Descripción del Proyecto

Este proyecto consiste en el desarrollo de una solución completa de análisis de datos para una empresa ficticia de e-commerce internacional llamada **DaniMarket**.

El objetivo principal es analizar:

- 📈 Ventas
- 💰 Beneficios
- 📦 Pedidos
- 🌍 Rendimiento geográfico
- 🛒 Categorías y productos

entre los años **2021 y 2024**, utilizando tecnologías modernas de **Big Data**, arquitectura **Lakehouse** y visualización interactiva con **Power BI**.

El proyecto implementa una arquitectura tipo **Medallion Architecture**:

```text
Bronze → Silver → Gold
```

utilizando:

- ⚡ Apache Spark
- 🧱 Delta Lake
- 📊 Power BI

---

# 🎯 Objetivos del Proyecto

## Objetivo General

Desarrollar un pipeline completo de análisis de datos capaz de transformar datos brutos en información estratégica para la toma de decisiones empresariales.

---

## Objetivos Específicos

✅ Analizar evolución de ingresos y beneficios  
✅ Identificar productos y categorías más rentables  
✅ Evaluar comportamiento de pedidos y entregas  
✅ Analizar ventas por país y región  
✅ Construir KPIs ejecutivos  
✅ Crear dashboard interactivo en Power BI  
✅ Aplicar procesos ETL modernos con Spark y Delta Lake

---

# 🛠️ Tecnologías Utilizadas

## ⚙️ Procesamiento y ETL

| Tecnología | Uso |
|---|---|
| Apache Spark (Scala) | Procesamiento distribuido |
| Delta Lake | Arquitectura Lakehouse |
| VS Code | Desarrollo ETL |

---

## 📊 Visualización

| Tecnología | Uso |
|---|---|
| Power BI Desktop | Dashboard interactivo |

---

## 💾 Almacenamiento

| Formato | Uso |
|---|---|
| CSV | Datos fuente y exportaciones |
| JSON | Campañas de marketing |
| Delta Tables | Capas Bronze, Silver y Gold |

---

## 🔧 Herramientas Complementarias

- Git & GitHub
- Power Query
- Bing Maps
- Kaggle Dataset

---

# 🧱 Arquitectura del Proyecto

```text
Kaggle CSV + JSON generado
        ↓
Bronze: ingesta raw en Delta
        ↓
Silver: limpieza, tipos, nulos, duplicados, joins
        ↓
Gold: KPIs y agregaciones
        ↓
CSV exportado
        ↓
Power BI Dashboard
```

---

# 📂 Estructura del Proyecto

```text
proyecto_final_bigdata_scala/
├── dashboard/
│   ├── dashboard_bigdata.pbix
│   └── dashboard_preview.png
│
├── datos/
│   ├── orders_raw.csv
│   └── marketing_campaigns.json
│
├── etl/
│   ├── bronze_layer.ipynb
│   ├── silver_layer.ipynb
│   └── gold_layer.ipynb
│
├── delta/
│   ├── bronze/
│   ├── silver/
│   └── gold/
│
├── export_powerbi/
│   └── final_csv/
│
├── informe/
│   └── informe_proyecto.pdf
│
├── README.md
└── .gitignore
```

---

# 📥 Fuentes de Datos

## 📄 Dataset Principal

Archivo CSV descargado desde **Kaggle** con más de **10.000 registros** de ventas e-commerce.

### Información incluida:

- Pedidos
- Productos
- Categorías
- Países
- Ingresos
- Beneficios
- Estado de pedidos

---

## 📑 Dataset Secundario

Archivo JSON generado manualmente con información de campañas de marketing.

---

# 🥉 Bronze Layer

## Objetivo

Almacenar datos originales sin transformación.

### Procesos realizados

✅ Ingesta CSV  
✅ Ingesta JSON  
✅ Escritura en Delta Lake

---

# 🥈 Silver Layer

## Objetivo

Limpiar y transformar datos para análisis posteriores.

### Transformaciones aplicadas

✅ Conversión de tipos de datos  
✅ Eliminación de duplicados  
✅ Tratamiento de nulos  
✅ Estandarización de columnas  
✅ Integración mediante joins

---

# 🥇 Gold Layer

## Objetivo

Generar tablas analíticas optimizadas para reporting.

---

## 📌 KPIs Generados

| KPI | Descripción |
|---|---|
| 💰 Ingresos Totales | Total de ingresos generados |
| 📈 Beneficio Total | Beneficio neto acumulado |
| 📦 Pedidos Totales | Número total de pedidos |
| 📊 Margen Promedio | Margen medio de beneficio |
| 🚚 % Pedidos Entregados | Pedidos entregados correctamente |

---

## 📊 Agregaciones Generadas

- Ventas mensuales
- Ranking de productos
- Ventas por país
- Ventas por categoría
- Estado de pedidos

---

# 📊 Dashboard Power BI

El dashboard incluye:

✅ KPIs ejecutivos  
✅ Evolución mensual de ingresos  
✅ Pedidos por año  
✅ Top productos más vendidos  
✅ Mapa de ingresos por país  
✅ Estado de pedidos  
✅ Participación de ingresos por categoría  
✅ Segmentador interactivo por año

---

## 🖼️ Vista del Dashboard

![Dashboard](dashboard/dashboard_preview.png)

---

# 🔍 Principales Insights

## 📈 Hallazgos obtenidos

- 📌 2023 fue el año con mayor volumen de pedidos.
- 📚 Books & Media generó el mayor porcentaje de ingresos.
- 💻 Los productos tecnológicos dominaron las ventas.
- 🌍 Europa y Norteamérica concentraron gran parte de ingresos.
- 🚚 Más del 60% de los pedidos fueron entregados correctamente.

---

# ▶️ Cómo Ejecutar el Proyecto

## 1️⃣ Clonar repositorio

```bash
git clone https://github.com/AnalistaDanielLlado/proyecto_final_bigdata.git
```

---

## 2️⃣ Ejecutar ETL

Ejecutar notebooks/scripts en este orden:

```text
bronze_layer.ipynb
silver_layer.ipynb
gold_layer.ipynb
```

---

## 3️⃣ Exportar CSVs

Las tablas Gold se exportan automáticamente en:

```text
export_powerbi/final_csv/
```

---

## 4️⃣ Abrir Power BI

Abrir archivo:

```text
dashboard/dashboard_bigdata.pbix
```

Actualizar datos y visualizar dashboard.

---

# 👨‍💻 Autor

## Daniel Lladó

📍 Madrid, España  
📊 Data Analyst Junior  
🌱 Agricultural Engineer  

### 🔗 LinkedIn

https://www.linkedin.com/in/daniel-llad%C3%B3/

---

# ✅ Estado del Proyecto

🟢 Proyecto finalizado y funcional.

Incluye:

- Arquitectura Big Data
- ETL completo
- Lakehouse con Delta
- KPIs ejecutivos
- Dashboard interactivo
- Visualizaciones avanzadas
- Análisis de negocio

---

# ⭐ Proyecto Académico

Proyecto desarrollado como práctica final de procesamientos de Big Data y Scala orientado a entornos empresariales reales.
