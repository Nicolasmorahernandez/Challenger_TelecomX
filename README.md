# Challenger_TelecomX

Este proyecto realiza un análisis exploratorio y descriptivo de la **evasión de clientes** (Churn) en un dataset de TelecomX. Utilizando un notebook de Google Colab, se llevan a cabo los siguientes pasos:

## 📁 Estructura del Repositorio

```
├── data/
│   └── TelecomX_Data(1).json       # Datos originales en formato JSON
├── notebooks/
│   └── churn_analysis.ipynb        # Notebook principal con todo el flujo de trabajo
├── README.md                       # Este archivo
└── requirements.txt                # Dependencias del proyecto
```

## 🚀 Instalación y Requisitos

1. Clonar este repositorio:

   ```bash
   git clone https://github.com/Nicolasmorahernandez/Challenger_TelecomX
   cd churn-analysis
   ```
2. Instalar requerimientos (en entorno virtual recomendado):

   ```bash
   pip install -r requirements.txt
   ```

> **requirements.txt** incluye:
>
> ```
> pandas
> numpy
> matplotlib
> seaborn
> scipy
> jupyter
> ```

## 📝 Notebook Principal

Abrir `notebooks/churn_analysis.ipynb` en Google Colab o Jupyter:

1. **Carga y limpieza de datos**:

   * Lectura del JSON con `pd.json_normalize`.
   * Eliminación de filas con `Churn` faltante.
   * Unificación de tipos y creación de variables: `Churn_bin`, `Cuentas_Diarias`, `Num_Servicios`.
2. **Análisis exploratorio**:

   * **Distribución de churn:** Gráfico de torta con porcentaje y conteo.
   * **Categóricas:** Gráficos de torta por género, contrato, método de pago, etc.
   * **Numéricas:** Boxplots comparativos de tenure, cargo mensual, cargo total y cargo diario.
3. **Correlación**:

   * Cálculo de matriz de correlación para clientes activos.
   * Heatmap y tabla de correlaciones en Markdown.
4. **Conclusiones y recomendaciones**:

   * Insights principales sobre patrones de churn.
   * Sugerencias estratégicas para reducir la tasa de cancelación.

## 🎯 Principales Hallazgos

* **Tasa de Churn:** 26.5% de los clientes abandona el servicio.
* **Contratos Month-to-Month:** 88.6% de los churners.
* **Tenure:** Mediana de 10 meses en churners vs 38 meses en no-churners.
* **Cargos:** Los churners tienen mayor cargo diario y mensual en mediana.
* **Correlaciones:** Fuerte relación entre número de servicios y cargos.

## 📌 Uso

* Ejecutar el notebook paso a paso para reproducir análisis y gráficos.
* Ajustar la paleta de colores o configuraciones de gráficos según preferencias.
* Extender con modelos predictivos de churn (Machine Learning) utilizando las variables generadas.

## 🛡️ Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo `LICENSE` para más detalles.

---

*Creado por Tu Nombre - `nicolas@example.com`*
