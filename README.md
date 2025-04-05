# 🌱 GrowWise - Predicción de Producción Agrícola (PoC)

## Descripción

GrowWise es una prueba de concepto (POC) para un sistema de predicción de producción agrícola que integra datos climáticos históricos y datos de producción. Este proyecto demuestra la viabilidad de utilizar técnicas de Machine Learning para predecir la producción de diferentes cultivos basándose en patrones climáticos y datos históricos.
Desarrollado como parte del TFM (Trabajo Fin de Máster), esta POC explora la relación entre variables climáticas y producción agrícola,proporcionando un marco inicial para herramientas predictivas que podrían beneficiar a agricultores, investigadores y responsables de políticas agrícolas.

## Estado del Proyecto

Este repositorio contiene una **Prueba de Concepto** y no debe considerarse un producto terminado o listo para producción. Los modelos, metodologías y flujos de trabajo demuestran la viabilidad técnica del enfoque propuesto y pueden servir como base para desarrollos futuros más robustos.


## 📊 Fuentes de Datos

Las fuentes principales de datos utilizadas en este proyecto son:

- **Datos Climáticos**: [Global Temperature Report for 2024 - Berkeley Earth](http://berkeleyearth.org/global-temperature-report-for-2023/)
  - Series temporales de temperatura global y regional
  - Datos sobre extremos climáticos

- **Datos Agrícolas**: [Organización de las Naciones Unidas para la Alimentación y la Agricultura (FAO)](http://www.fao.org/statistics/es)
  - Producción agrícola por país/región
  - Área cosechada
  - Rendimientos por hectárea

## 🚀 Estructura del Proyecto

El proyecto está organizado en una serie de notebooks Jupyter que deben ejecutarse en el siguiente orden:

### 1. Transformación de Datos
- **`data_transformation.ipynb`**: Procesamiento inicial de datos agrícolas de la FAO
- **`data_transformation_temperaturas.ipynb`**: Transformación de datos climáticos
- **`data_temp.ipynb`**: Procesamiento adicional de datos de temperatura

### 2. Análisis y Fusión de Datos
- **`data_merge_and_analysis.ipynb`**: Integración de datos climáticos y agrícolas, análisis exploratorio

### 3. Modelado Predictivo
- **`Prediction_modelV2.ipynb`**: Implementación de modelos de Machine Learning para la predicción de producción agrícola

### 4. Visualización
- Los resultados finales son exportados para su visualización en Power BI, generando un dashboard interactivo de alto impacto.

## 📂 Estructura de Carpetas

- **notebooks/** - Notebooks Jupyter
- **data/** - Datos de origen y transformados
  - **raw/** - Datos originales sin procesar
  - **processed/** - Datos procesados y listos para modelado
- **models/** - Modelos entrenados
- **power_bi/** - Archivos para Power BI
- **README.md** - Este archivo

## 💻 Tecnologías Utilizadas

- **Python**: Procesamiento de datos y modelado
- **Pandas/NumPy**: Manipulación y análisis de datos
- **os/pathlib**: Gestión de rutas y archivos del sistema
- **Scikit-learn**: Implementación de modelos de Machine Learning
- **XGBoost**: Modelado avanzado con Gradient Boosting
- **Matplotlib/Seaborn**: Visualización de datos
- **Power BI**: Creación de dashboard interactivo

## 📈 Modelos Implementados

El proyecto implementa y compara varios modelos de Machine Learning:

1. **Linear Regression (Baseline)**: Modelo básico como punto de referencia
2. **Ridge Regression**: Regresión regularizada para evitar sobreajuste
3. **Random Forest**: Conjunto de árboles de decisión para capturas relaciones complejas
4. **Gradient Boosting**: Modelo de boosting para mejorar la precisión predictiva
5. **XGBoost**: Implementación eficiente de Gradient Boosting

Cada modelo es evaluado mediante validación cruzada temporal, respetando la estructura cronológica de los datos.

## 🔍 Características Principales

- Integración de datos climáticos y agrícolas
- Series temporales con datos históricos (lag features)
- Validación cruzada temporal
- Optimización de hiperparámetros
- Análisis de importancia de características
- Visualización interactiva en Power BI

## 📊 Resultados y Visualización
El resultado final del proyecto es un dashboard interactivo en Power BI que permite explorar predicciones de producción por cultivo, analizar tendencias y visualizar el impacto de diferentes variables climáticas.


© 2025 GrowWise | Desarrollado como parte del TFM - Máster en Big Data & Analytics EAE Business School Barcelona
