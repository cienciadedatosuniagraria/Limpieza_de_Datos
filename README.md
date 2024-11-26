### Limpieza de Datos del Titanic: Un Notebook Esencial

Este repositorio contiene un Jupyter Notebook que implementa un proceso completo de limpieza de datos utilizando el conocido dataset Titanic, disponible a través de la biblioteca seaborn. El objetivo es guiarte paso a paso en la preparación de datos limpios y estructurados, listos para análisis o modelado.

Contenido del Notebook
El notebook incluye las siguientes secciones:

I. Descripción del Dataset Titanic
El dataset contiene información detallada sobre los pasajeros del Titanic, incluyendo:

Variables relevantes como survived, pclass, sex, age, entre otras.
Detalles sobre la estructura del dataset y los valores que representa cada columna.
Se proporciona una descripción exhaustiva de cada campo para facilitar su comprensión.

II. Proceso de Limpieza
La limpieza de datos incluye los siguientes pasos:

Importación de Bibliotecas y Dataset
Cargar el dataset desde seaborn y mostrar una vista previa de los datos.

Exploración Inicial
Inspeccionar el dataset para identificar valores nulos, tipos de datos y estructura general.

Tratamiento de Valores Faltantes

Rellenar valores numéricos (como age) con la mediana.
Completar valores categóricos (como embarked) con la moda.
Eliminar columnas con demasiados valores faltantes, como deck.
Corrección de Tipos de Datos
Convertir variables como sex y embarked a tipos categóricos para ahorrar memoria y optimizar análisis.

Eliminación de Datos Duplicados
Identificar y eliminar filas duplicadas para garantizar integridad.

Normalización y Transformación

Escalar valores numéricos (fare) entre 0 y 1.
Codificar variables categóricas (sex, embarked) en variables dummy con pd.get_dummies.
Validación Final
Verificar que no queden valores nulos y obtener una vista previa del dataset limpio.

Exportación del Dataset Limpio
Guardar el dataset final en formato CSV (titanic_limpio.csv) para su uso en futuros análisis o proyectos.
