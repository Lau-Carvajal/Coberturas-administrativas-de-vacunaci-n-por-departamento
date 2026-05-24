# Coberturas administrativas de vacunación por departamento

## Descripción 

El dataset contiene datos de cobertura de vacunación por departamento en Colombia, mostrando el avance porcentual en la aplicación de distintos biológicos del esquema nacional de vacunación. Esta información permite analizar qué departamentos presentan mayores o menores niveles de cobertura y sirve como apoyo para estudios de salud pública.

## Integrantes 

- Nicólas Barbosa
- Laura Carvajal

## Dataset

- Fuente: datos.gov.co
- Nombre del dataset: Coberturas administrativas de vacunación por departamento
- Link: https://www.datos.gov.co/Salud-y-Protecci-n-Social/Coberturas-administrativas-de-vacunaci-n-por-depar/6i25-2hdt/about_data
- Variables: 12 variables y 660 registros

## Tecnologías usadas

- Python, PyCaret, Streamlit y GitHub

## Estructura del repositorio

- Notebook.ipynb → Análisis y modelos
- App.py → Aplicación Streamlit
- Requirements.txt → Librerías necesarias
- Datos/ → Dataset del proyecto


## ¿Cómo correr la App?

1. pip install -r requirements.txt
2. streamlit run app.py

## Resultados
A partir del análisis exploratorio del dataset y de la clasificación realizada con los modelos de Regresión Logística y Árbol de Decisión, se identificó que los departamentos con mayor cobertura promedio fueron Atlántico, Arauca, La Guajira, Guainía, Casanare y Sucre. Estos departamentos presentaron mejores niveles promedio de cobertura frente a otros territorios del país.

En cuanto a los biológicos, las vacunas con mayor cobertura promedio fueron la Triple Viral al año, BCG y PENTA3. Esto puede explicarse porque hacen parte de esquemas de vacunación infantil con mayor seguimiento institucional, especialmente en edades tempranas.

Es importante aclarar que los modelos de Machine Learning permiten clasificar los niveles de cobertura, pero la identificación de los departamentos y vacunas con mayor cobertura se obtiene principalmente mediante el análisis exploratorio y la agrupación de los datos. Los modelos ayudan a confirmar que variables como el departamento, el año y el tipo de biológico influyen en la clasificación del nivel de cobertura.

## Conclusión de resultados

A partir de los resultados obtenidos con el modelo de Regresión Logística y el modelo de Árbol de Decisión, se puede observar que ambos modelos permiten realizar una clasificación del nivel de cobertura de vacunación por departamento, año y biológico. Sin embargo, su comportamiento puede variar dependiendo de la capacidad de cada algoritmo para identificar patrones dentro de los datos.

La Regresión Logística funciona como un modelo base, ya que permite tener una primera referencia del desempeño del proyecto. Este modelo es más simple y fácil de interpretar, pero puede presentar limitaciones cuando las relaciones entre las variables no son completamente lineales.

Por otra parte, el Árbol de Decisión permite construir reglas más claras a partir de las variables del dataset, lo que facilita la interpretación de los resultados. Este modelo puede identificar relaciones más específicas entre el departamento, el año y el biológico, por lo que resulta útil para explicar cómo se clasifican los niveles de cobertura.

En términos generales, los resultados muestran que las variables territoriales y el tipo de biológico pueden influir en la clasificación del nivel de cobertura. Esto permite evidenciar que la cobertura de vacunación no se comporta de la misma manera en todos los departamentos ni para todos los biológicos, lo cual es importante desde una perspectiva de salud pública.

Estos primeros modelos permiten avanzar en la comparación de algoritmos de Machine Learning. Posteriormente, al incluir modelos como Random Forest y XGBoost, será posible evaluar si algoritmos más robustos logran mejorar las métricas de clasificación, especialmente el Accuracy, Precision, Recall y F1 Score.

En conclusión, el análisis inicial demuestra que el dataset sí contiene información útil para clasificar los niveles de cobertura de vacunación y que los modelos de Machine Learning pueden servir como herramienta de apoyo para identificar diferencias en el comportamiento de la vacunación por departamento en Colombia.
