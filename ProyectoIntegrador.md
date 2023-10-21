<center><h1>Reporte Proyecto Integrador </h1></center>

## Introduccion:

En este proyecto, se tenia por objetivo realizar un moodelo que fuera capaz de predecir si una persona era caso o no de una cierta enfermedad, para esto contamos con un datasets, donde teniamos infromacion de distintos pacientes, el cual fue trabajado para el desarrollo.

## EDA:

La primera etapa de este proyecto, consto de un procesos de exploracion de los datos, proceso en el cual se realizaron tareas, como analizar las distribuciones de variables numericas, para descubrir valores atipicos, e histogramas para variables categoricas.
Ademas, se eliminaron columnas que no se considerarian para el analisis, se realizaron trasnformaciones en los datos, tales como eliminar registros con nulos, imputacion de valores faltantes, y normalizacion todo esto en cuanto corresponderia segun el criterio basado en la informacion que se tenia.

## Preparacion de los datos:

En este proyceso, con los datos ya limpios, se procedio a preparar los datos para el analisis (complementar lo ya realizado), en este pasos, se generaron variables dummies para campos en los cuales correspondiere, y se realizo una binarizacion para otros.

## Modelado:

Con los datos ya listos, se procedio al modelado, para esto el dataset fue separado en uno de train y uno de test. Para este primero, se realizo una validacion cruzada con tres modelos distintos, Arbol de decision, Vecinos cercanos, y Bosque Ramdom, luego se procedio a analizar los scores de cada uno, dando que, el modelo de Bosque Ramdom fue el mas optimo. Teniendo este modelo se realizo un GridSearch para seleccionar los estimadores mas optimos.
Con el modelo y sus mejores hiperparametros, se procedio a usar el dataset de test para testearlo. y calcular sus metricas.

## Conclusion:

Para poder realizar conclusiones de este modelo, se seleccionaron metricas que estuvieran acorde al estudio a realizar, una de las mas importantes seria la sensibilidad, ya que daria un indice de los falsos negativos(personas caso que se predicen como sanas), este valor dio un numero bastante bajo y a pesar de otras metricas dieren mas altas, no es un dato menor.
Por esto se puede concluir que si bien el modelo parece tener un cierto nivel de predictibilidad, no puede usarse solo como referencia para predecir este tipo de enfermedad, deberia complementarse con otros estudios, o obtener nuevos datos con variables distintas.


