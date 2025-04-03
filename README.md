# Dashboard interactivo vehiculos vendidos en Uruguay 2024

**ETL**:
Para poder analizar los datos, tuve que limpiar la base de datos ya que contenia informacion que no iba a utilizar por lo que tuve que eliminar "IMESI, cantidad de puertas del vehiculo, cilindradas, etc). Esta informacion no me parecia relevante.
Luego se me presento el problema de que la base de datos estaba filtrada por mes y cantidad total. Por lo que a la hora de cargarlo en Power BI, este mismo, no me lo reconocia como un mes sino que lo consideraba un texto general. Esto me iba a traer muchos problemas a la hora de querer filtrar la informacion con slicers y filtros varios en el dashboard.

Para poder solucionar este asunto seleccione las columnas de enero a octubre y las despivotee. Con esta funcion me quedaba descriminado cada mes en una columna y la cantidad en otra columna. Luego de solucionar este problema, persistia el no poder filtrar por mes en el dashboard. Por lo que tuve que agregar una columna en Power Query que me ordene los meses por orden numerico (1 al 12) y no por orden alfabetico (abril, agosto...). Una vez agregada esta columna asocie en el modelado la columna del mes con la columna "mes numero" y ordene la misma por el orden numerico agregado. 

**COMENTARIOS FINALES**
En Uruguay se vendieron un total de 50.000 autos 0 KM de enero a octubre. El tipo de vehiculo mas vendido fue el auto sedan/hatchback, los cuales continuan siendo los mas fuertes entre todos los segmentos. Por otro lado continua en alza la venta de SUV, no es noticia saber que ultimamente se ven muchos vehiculos con este tipo de carroceria. Por otro lado podemos observar que los vehiculos mas vendidos continuan siendo el combustible a nafta o diesel. Si bien aumentaron considerablemente la venta de autos electricos e hibridos, estos aun continuan muy por debajo de los autos nafteros. 

El principal proveedor de estos autos vendidos son Brasil, Chile, Argentina, India y Mexico. El acuerdo del mercosur entre Argentina y Brasil surge efecto ya que posibilita la obtencion de vehiculos de dichos origines por costos mas bajos que sus competidores en Europa o Asia. Cabe destacar que el 100% de los vehiculos importados de Chile son electricos o hibridos, esto se debe al bajo costo que tiene producir las baterias de litio en dicho pais. 
