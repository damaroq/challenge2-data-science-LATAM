# Proyecto ETL y Análisis de Evasión de Clientes (Churn) — Telecom X

## 📌 Descripción
Este proyecto tiene como objetivo analizar la **evasión de clientes (Churn)** en la empresa ficticia **Telecom X**, utilizando un enfoque **ETL (Extract, Transform, Load)** y un análisis exploratorio de datos (EDA).  

El dataset fue provisto en formato **JSON** (simulando la extracción desde una API) y contiene información demográfica, servicios contratados y métricas de facturación de los clientes.  

A partir del análisis, se busca identificar **patrones y factores asociados al abandono de clientes**, para proponer **estrategias de retención** que ayuden a reducir la tasa de churn.

---

## 🗂️ Estructura del Proyecto
El flujo de trabajo sigue la metodología **ETL + Análisis**:

1. **Extracción (E - Extract)**  
   - Lectura de datos desde archivo JSON (simulando una API).  
   - Conversión de los datos a un DataFrame de Pandas.  

2. **Transformación (T - Transform)**  
   - Exploración de columnas y tipos de datos.  
   - Limpieza: tratamiento de valores nulos, duplicados e inconsistencias.  
   - Conversión de variables categóricas (ej. `"Yes"/"No"` → `1/0`).  
   - Creación de nuevas variables, como `Cuentas_Diarias` (costo mensual dividido entre 30).  

3. **Carga y Análisis (L - Load & Analysis)**  
   - Análisis descriptivo: media, mediana, desviación estándar y estadísticas de variables relevantes.  
   - Distribución del churn global mediante gráficos.  
   - Análisis de churn por variables categóricas (ej. contrato, método de pago, internet).  
   - Análisis de churn por variables numéricas (ej. tenure, cargos mensuales, total gastado).  
   - Obtención de **insights clave** sobre patrones de abandono.  

4. **Informe Final**  
   - Incluye introducción, limpieza de datos, análisis exploratorio, conclusiones e insights, y recomendaciones estratégicas.  
   - Todas las secciones están documentadas dentro del mismo Notebook en celdas de texto y visualizaciones.  

---

## 📦 Requisitos
El proyecto se desarrolló en **Google Colab** con las siguientes librerías:

`bash`
`pandas`
`numpy`
`matplotlib`
`seaborn`

## 🚀 Ejecución

1. Abrir el notebook en Google Colab.

2. Cargar el archivo TelecomX_Data.json en el entorno de Colab.

3. Ejecutar las celdas en orden:

4. Extracción de datos

5. Transformación

6. Carga y Análisis

## Informe final

**📈 Resultados Principales**

- Se identificó que la tasa global de churn es significativa en clientes con:

- Contratos de tipo mensual.

- Métodos de pago como electronic check.

- Servicios de Internet con fibra óptica.

- Clientes con tenure bajo (primeros 12 meses).

- Cargos mensuales altos.

- La creación de la variable Cuentas_Diarias permitió observar comportamientos más detallados en el gasto promedio diario.

## 🎯 Recomendaciones Estratégicas

- Incentivar contratos de largo plazo con promociones o descuentos.

- Mejorar la experiencia de facturación y diversificar métodos de pago.

- Implementar programas de onboarding y fidelización en los primeros meses.

- Diseñar planes personalizados para clientes con cargos elevados.

- Fortalecer la calidad del servicio de internet y soporte técnico.

## 📝 Autor

Proyecto desarrollado por Deyci Amaro Quispe
