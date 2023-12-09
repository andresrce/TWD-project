# Título del Proyecto: Análisis de la Popularidad de TWD
# Contextualización de la Serie
# Introducción a "The Walking Dead":
"The Walking Dead" es una serie de televisión de gran impacto basada en el cómic homónimo. Lanzada en 2010, narra la historia de supervivientes en un mundo post-apocalíptico plagado de zombis. La serie es conocida por su intensa trama y personajes complejos, capturando la atención de audiencias a nivel mundial.

# Datos Utilizados:
El conjunto de datos incluye información detallada de cada episodio desde la primera hasta la última temporada emitida. Contiene datos sobre la temporada, número de episodio, título, director, escritor, fecha de emisión original y audiencia en millones de espectadores en Estados Unidos.
Dataset "The Walking Dead Episodes": https://www.kaggle.com/datasets/abdurrakibmollah/the-walking-dead-episodes (scrapeado de Wikipedia)

# Preguntas Guía
¿Cómo ha evolucionado la popularidad de "The Walking Dead" a lo largo de las temporadas y episodios?
¿Cuál es la influencia de los directores y escritores en la popularidad de los episodios?

# Metodología

## Preparación de Datos:
Se realizó una limpieza y preparación de los datos, incluyendo la conversión de fechas y la codificación de variables categóricas como los nombres de directores y escritores.

## Análisis Visual:
Se visualizó la audiencia promedio por temporada para identificar tendencias generales de popularidad.
Se usó un gráfico de cajas para examinar la distribución de la audiencia por temporada.
Se elaboraron gráficos de línea para mostrar la evolución de la audiencia en cada episodio y a lo largo del tiempo.
Se marcó la audiencia en episodios con eventos clave de la trama para analizar su impacto en la popularidad.

## Análisis de Directores:
Se aplicó codificación one-hot para los nombres de los directores.
Se utilizó un modelo de regresión de Random Forest, entrenado con los datos de los directores.
El modelo fue evaluado usando RMSE (0.752 millones de espectadores) y R^2 (0.968), indicando alta precisión en la predicción de la audiencia.

# Conclusiones
## Popularidad de la Serie:
- La audiencia ha mostrado variaciones notables a lo largo de las temporadas, con picos y caídas que podrían estar asociados a eventos importantes en la trama y cambios en el elenco.
- Las visualizaciones destacan cómo momentos específicos, como la muerte de personajes importantes o enfrentamientos clave, afectaron la popularidad del programa.
## Influencia de Directores en la Popularidad: 
- El modelo de regresión demostró ser eficaz en predecir la audiencia basada en los directores de los episodios.
- Los resultados sugieren que los directores tienen un impacto significativo en la popularidad de los episodios.
- Se identificaron limitaciones como la exclusión de otros factores potenciales y la generalización de los resultados.
