# Limpieza de Datos del Titanic: Un Notebook Esencial

Este repositorio contiene un **Jupyter Notebook** diseñado para realizar un proceso completo de limpieza de datos utilizando el dataset Titanic, ampliamente reconocido por su relevancia en análisis de datos. Este notebook es ideal para aprender a preparar datos de manera estructurada y eficiente, dejándolos listos para análisis o modelado.

## Contenido del Notebook

### **1. Descripción del Dataset Titanic**
- El dataset incluye información detallada sobre los pasajeros del Titanic, como:
  - **Variables principales:** `survived`, `pclass`, `sex`, `age`, entre otras.
  - **Estructura:** Detalles sobre cada columna y los valores que representa.
- Se presenta una descripción exhaustiva de los datos para facilitar su comprensión.

---

### **2. Proceso de Limpieza**
El proceso de limpieza incluye los pasos esenciales para transformar datos en su estado más útil:

#### **a. Importación de Bibliotecas y Dataset**
- Carga del dataset directamente desde la biblioteca `seaborn`.
- Vista previa inicial para comprender su estructura.

#### **b. Exploración Inicial**
- Identificación de:
  - Valores nulos.
  - Tipos de datos.
  - Estadísticas descriptivas y estructura general.

#### **c. Tratamiento de Valores Faltantes**
- Rellenar valores numéricos (`age`) con la **mediana**.
- Completar valores categóricos (`embarked`) con la **moda**.
- Eliminar columnas con alta proporción de valores faltantes (`deck`).

#### **d. Corrección de Tipos de Datos**
- Conversión de variables categóricas como `sex` y `embarked` a **tipos categóricos** para optimizar memoria y análisis.

#### **e. Eliminación de Datos Duplicados**
- Identificación y eliminación de filas duplicadas para garantizar la integridad del dataset.

#### **f. Normalización y Transformación**
- Escalado de valores numéricos (`fare`) entre 0 y 1.
- Codificación de variables categóricas (`sex`, `embarked`) mediante **variables dummy** con `pd.get_dummies`.

#### **g. Validación Final**
- Verificación de la limpieza del dataset:
  - Confirmar ausencia de valores nulos.
  - Inspeccionar las primeras filas del dataset final.

---

### **3. Exportación del Dataset Limpio**
- El dataset limpio se guarda en formato **CSV** (`titanic_limpio.csv`) para facilitar su uso en futuros proyectos o análisis.

---

## ¿Por qué usar este Notebook?
- **Educación práctica:** Aprender técnicas de limpieza de datos paso a paso.
- **Aplicación directa:** Preparar datos reales para análisis estadístico, modelado o visualización.
- **Reutilización:** Exportar un dataset limpio y estructurado para futuros proyectos.

---

## Requisitos
- **Python 3.x**
- Bibliotecas necesarias:
  - `pandas`
  - `numpy`
  - `seaborn`

Instala las dependencias con:
```bash
pip install pandas numpy seaborn
