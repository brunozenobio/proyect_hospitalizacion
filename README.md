# proyect_hospitalizacion

## Introducción

El objetivo de este proyecto fue desarrollar un modelo capaz de predecir si una persona era un caso de cierta enfermedad. Para esto, se utilizó un conjunto de datos que contenía información de diferentes pacientes. A lo largo del proyecto, se llevaron a cabo diversas etapas de procesamiento y análisis de datos para desarrollar el modelo predictivo.

## Exploración de Datos (EDA)

La primera fase del proyecto consistió en explorar los datos. Se realizaron análisis de las distribuciones de variables numéricas para identificar valores atípicos y se crearon histogramas para variables categóricas. Además, se eliminaron columnas irrelevantes, se realizaron transformaciones como la eliminación de registros nulos, imputación de valores faltantes y normalización, según fuera necesario basándose en la información disponible.

## Preparación de los Datos

Con los datos limpios, se procedió a prepararlos para el análisis adicional. Se crearon variables dummy para ciertos campos y se aplicó binarización en otros, según fuera necesario.

## Modelado

Una vez que los datos estuvieron listos, se procedió al modelado. El conjunto de datos se dividió en conjuntos de entrenamiento y prueba. Se aplicó validación cruzada con tres modelos diferentes: Árbol de decisión, Vecinos cercanos y Bosque Aleatorio. Después de comparar los puntajes, el modelo de Bosque Aleatorio demostró ser el más óptimo. Se utilizó GridSearch para seleccionar los hiperparámetros óptimos para este modelo. Posteriormente, se evaluó el modelo con el conjunto de prueba y se calcularon las métricas correspondientes.

## Conclusiones

Al evaluar el modelo, se seleccionaron métricas adecuadas para el estudio, siendo la sensibilidad una de las más importantes, ya que proporciona un indicador de los falsos negativos (personas enfermas que se predicen como sanas). A pesar de que otras métricas mostraron valores más altos, la sensibilidad fue baja, lo cual es preocupante. En conclusión, aunque el modelo parece tener cierto nivel de predictibilidad, no se puede utilizar como única referencia para predecir esta enfermedad. Sería necesario complementarlo con otros estudios o recopilar nuevos datos con variables diferentes para mejorar su desempeño y confiabilidad.
