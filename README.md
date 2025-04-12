# PnLVisualizer

Esta aplicación interactiva desarrollada con Shiny implementa el modelo de Black-Scholes para calcular precios de opciones europeas tipo Call y Put. A través de un panel amigable e intuitivo, permite explorar cómo cambian los precios y las ganancias/pérdidas esperadas (PnL) ante variaciones en parámetros clave como el precio spot y la volatilidad. La app incluye visualizaciones dinámicas mediante heatmaps, y cuenta con conexión a una base de datos MySQL, donde se almacenan automáticamente los inputs y resultados de cada simulación para facilitar su trazabilidad y análisis posterior.

http://038p5o-jesus-martinez.shinyapps.io/pet1

## 📂 Contenido del repositorio

- `app/`: versión lista para ser deployada en shinyapps.io.
- `app_db/`: versión avanzada que incluye conexión a base de datos.
- `sql/schema.sql`: queries para crear y poblar las tablas necesarias.
- `README.md`: esta documentación.

## 🚀 Funcionalidades

### 1. Cálculo y simulación de opciones

- Cálculo de precios de opciones europeas (Call y Put) mediante el modelo de Black-Scholes.
- Simulación de compra y venta con cálculo de PnL (ganancias/pérdidas).
- Visualización en tiempo real de precios Call y Put.

### 2. Dashboard interactivo

- Panel para ingresar parámetros clave: Spot (S), Strike (K), Tiempo al vencimiento (T), Volatilidad (σ) y Tasa libre de riesgo (r).
- Configuración de rangos personalizados para generar heatmaps.
- Heatmaps dinámicos de precios y PnL bajo distintos escenarios.
- Botón para restablecer parámetros a valores predeterminados.

### 3. Persistencia en base de datos

- Registro automático de cada simulación en una base de datos MySQL.
- Guardado estructurado de inputs, outputs y shocks relativos (spot y volatilidad).

## ⚙️ Escalabilidad

Aunque esta aplicación está actualmente conectada a una base de datos MySQL, su arquitectura permite adaptarla fácilmente a otros sistemas de almacenamiento como PostgreSQL, SQLite, o servicios en la nube como Amazon RDS, Google Cloud SQL o Azure SQL Database.

