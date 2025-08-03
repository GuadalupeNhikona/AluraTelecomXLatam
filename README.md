# 📊 AluraTelecomXLatam

Análisis de evasión de clientes en el sector de telecomunicaciones utilizando Python y técnicas de ETL. Proyecto realizado como parte del Challenge de Data Science para LATAM con Alura.

## 📌 Objetivo

Identificar patrones en la fuga de clientes (“Churn”) de una empresa de telecomunicaciones, empleando técnicas de extracción, transformación y análisis de datos.

## ⚙️ Tecnologías utilizadas

- Python (Google Colab)
- Pandas
- Numpy
- Requests
- JSON

## 🔍 Proceso ETL

### 1. **Extracción**
- Se utilizó un archivo JSON alojado en GitHub como fuente de datos:  
  [TelecomX_Data.json](https://raw.githubusercontent.com/alura-cursos/challenge2-data-science-LATAM/main/TelecomX_Data.json)
- Se verificó la conexión y se cargó el archivo exitosamente.

### 2. **Transformación**
- Normalización de campos con diccionarios anidados (`customer`, `phone`, `internet`, `account`)
- Uso de `explode()` para listas internas
- Conversión de columnas tipo `object` a `string`
- Verificación de integridad y consistencia de datos

### 3. **Carga**
- Los datos transformados quedaron listos para análisis exploratorio, modelado predictivo y visualización.

## 🧠 Diccionario de datos

- `customerID`: ID único del cliente  
- `Churn`: ¿Abandonó o no la empresa?  
- `gender`, `SeniorCitizen`, `Partner`, `Dependents`, `tenure`: variables demográficas  
- `PhoneService`, `MultipleLines`, `InternetService`, etc.: servicios contratados  
- `Charges.Monthly`, `Charges.Total`: monto mensual y total gastado

## 📈 Resultados esperados

- Comprender los factores que influyen en la evasión de clientes.
- Generar modelos predictivos o insights que ayuden a mejorar la retención.

## 🙌 Créditos

Este proyecto forma parte del Challenge TelecomX organizado por Alura Latam.  
Autora: Guadalupe Nhikona
