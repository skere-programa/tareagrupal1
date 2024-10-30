# tareagrupal1
Resolución de los problemas con Geodatframe
EJERCICIO 1: Se tomó un mapa sin proyección (también conocido como "datos sin CRS" o sistema de referencia de coordenadas) y se le asignó un sistema de referencia adecuado. Una vez proyectado, se calculó el centroide del país. De ello se obtuvieron las capas de las ciudades y ríos del país usando el centroide como referencia o como un punto clave en el análisis.

EJERCICIO 2: Obtuvimos inicialmente la informacion de los aeropuertos de Rusia  en formato de DataFrame. Para proyectar los aeropuertos en el mapa del país, convertimos este DataFrame a un GeoDataFrame, lo que permitió trabajar con coordenadas y realizar visualizaciones geográficas.

EJERCICIO 3:Primero vemos si Rusia proyectado es un multipolígono; ahora con el país proyectado, vamos a mostrar el borde del país con Boundary y finalmente, convertimos a un geodataframe en vez de una geoserie y creamos una nueva columna con nombre del país, además que la columna Geometry sea la columna de geometría

EJERCICIO 4: Primero, subimos archivos de estados y municipalidades al GitHub y en raw copiamos los links tanto para los states como para las municipalities; ambos son geodataframe y geometry; en nuestro caso sí tiene CRS y ya no es necesario hacer nada. Si no tuviera CRS, lo que hacemos es el crs de state y municipalitie lo establecemos como un no proyectado con "EPSG y con número del país sin proyectar", luego proyectamos con .to_crs ("número del país proyectado")

EJERCICIO 5: En este problema, primero cargamos una tabla llamada FRAGILITYCIA y comparamos los nombres de los países con la tabla countries para asegurar que coincidieran. Luego, tomamos las variables CO2 y FORESTREV_gdp de FRAGILITYCIA y las reescalamos para hacerlas comparables, permitiendo observar qué países tienen mayores o menores niveles de emisiones de CO2 y de ingresos forestales. Posteriormente, clasificamos estos valores en una escala del 1 al 4 y, finalmente, generamos un mapa mundial que muestra visualmente esta clasificación para facilitar la comparación entre países.

https://skere-programa.github.io/tareagrupal1/
