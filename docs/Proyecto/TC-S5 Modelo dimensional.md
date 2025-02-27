# **Modelo dimensional del proyecto y diseño del proceso ETL**
## **Objetivo**
- Modelar multidimensionalmente la base datos (BD) utilizada para los análisis sugeridos del proyecto.  
- Diseñar el proceso ETL para cargar las tablas que se deben crear asociadas al modelo multidimensional propuesto.
## **Instrucciones**

![](Img/S210InfrestructuraVisible.png)


En esta fase del proyecto, a partir de los análisis requeridos y de fuentes de datos proporcionadas, Infraestructura Visible le solicita:
1.	**Entregable 1- Modelo multidimensional:** Una propuesta de modelo multidimensional que permita realizar los análisis propuestos que su grupo eligió, acompañado de una descripción y justificación del mismo. Suponga como proceso de negocio <i>RegistroDeVuelos</i> que se realiza de forma mensual.
2.	**Entregable 2 - Diseño del proceso ETL:** Incluir el diseño ETL propuesto para poblar las tablas asociadas al modelo multidimensional propuesto, utilizando como fuentes, las compartidas. Incluya una descripción general con los elementos que considere son importantes para la comprensión del diseño.

A continuación, se presentan los análisis propuestos y los datos requeridos para lograr los objetivos de esta tarea.

| Tema analítico  | Análisis requeridos o inferidos | Categoría del análisis (*)  | Procesos de negocio | Fuentes de datos |
| ------------- | ------------- | ------------- | ------------- | ------------- | 
| Comportamiento de vuelos y aeropuertos en Colombia   | Análisis 1 <br> a. Visualizar el número de pasajeros transportados (entrantes y salientes) en un rango de fechas. <br> b. Visualizar el número de pasajeros transportados (entrantes y salientes) en un rango de fechas de aeropuertos Internacionales a aeropuertos en Colombia o entre aeropuertos nacionales. <br> c. Visualizar el número de pasajeros transportados (entrantes y salientes) en un rango de fechas por departamento y país  | Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia  | Aeropuertos, Vuelos |
| Comportamiento de vuelos y aeropuertos en Colombia   | Análisis 2 <br> Visualizar el número de puestos desaprovechados en un rango de fechas de aeropuertos Internacionales a aeropuertos en Colombia o entre aeropuertos nacionales, los aeropuertos se pueden agrupar por departamento, país, etc  | Tablero de control  |  Tráfico y capacidad de carga aérea en aeropuertos de Colombia  | Aeropuertos, Vuelos |
| Comportamiento de vuelos y aeropuertos en Colombia   | Análisis 3 <br> Visualizar la carga transportada (entrante y saliente) en un rango de fechas de aeropuertos Internacionales a aeropuertos en Colombia o entre aeropuertos nacionales, los aeropuertos se pueden agrupar por departamento, país, etc  | Tablero de control  |  Tráfico y capacidad de carga aérea en aeropuertos de Colombia  | Aeropuertos, Vuelos |
| Comportamiento de vuelos y aeropuertos en Colombia   | Análisis 4 <br> Visualizar la carga desaprovechada en un rango de fechas de aeropuertos Internacionales a aeropuertos en Colombia o entre aeropuertos nacionales, los aeropuertos se pueden agrupar por departamento, país, etc  | Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia  | Aeropuertos, Vuelos |
| Comportamiento de vuelos y aeropuertos en Colombia   | Análisis 5 <br> Visualizar la información de los aeropuertos que están en centros poblados donde la población de mujeres es mayor a la de hombres, con un PIB, el año de análisis, superior al promedio del Departamento donde está el centro poblado y donde el número de vuelos por mes de un año particular seleccionado está por debajo del promedio nacional ese mismo mes de ese año. <br>| Tablero de control  | Tráfico y capacidad de carga aérea en aeropuertos de Colombia  | Aeropuertos, Vuelos  |
| Comportamiento de vuelos y aeropuertos en Colombia   | Análisis 6 <br> Visualizar la información de los aeropuertos y/o vuelos en relación a las proyecciones de habitantes por género, edad y pib <br>| Tablero de control  | Caracterización de los servicios vs comportamiento de los clientes |PIB,  Proyecciones de habitantes por edad y género  |

** Los análisis de la tabla pueden ser agrupaciones de análisis más pequeños o se pueden extender, incluso puede que los análisis no estén completos. Es libre de proponerle nuevos análisis al negocio o complementar los de la tabla como parte de sus conclusiones. Piense en que le beneficiaría más a Infraestructura Visible y en paticular a un usuario que esté interesado en este estilo de análisis.

## **Recursos requeridos**
***Datos suministrados***

Los datos los puede encontrar en la base de datos: ProyectoTransaccional del servidor que manejamos en los tutoriales. También puede encontrar el diccionario de los mismos [aquí](https://github.com/MISW-4402-Analisis-y-Modelado-de-datos/guias/blob/main/docs/Proyecto/Diccionario%20IV.xlsx), ambos recursos requeridos para el desarrollo de esta tarea, las tablas son copias de las tablas relacionales del negocio. 
-	aeropuertosCopia
-	divipolaCopia
-	vuelosCopia
-	pibCopia
-	proyeccionesCopia

***Tecnología***

Recuerde los videos y lecturas de modelado multidimensional, que serán de utilidad para el desarrollo de esta tarea.

Adicionalmente, se le sugiere utilizar una herramienta como [GenMyModel](https://www.genmymodel.com/) o [Lucidchart](https://lucid.app/es/users/login#/login?_gl=1*1sru4v4*_ga*MjA1NjkyODI5LjE2NTUzMjA2MzY.*_ga_MPV5H3XMB5*MTY1NTQzMTAyOS4yLjAuMTY1NTQzMTAyOS42MA..&anonId=0.8bb37e0e18168cc6c65&sessionDate=2022-06-17T01:57:06.970Z&sessionId=0.88d2ce41816f60d91a&activate=lucidchart) para dibujar el modelo. Este tipo de herramientas facilita el mantenimiento de los modelos de datos.

## **Recomendaciones de los entregables**
Incluir en la entrega la dirección (URL) de la wiki de su repostiro <i>Estudiante_i</i> donde registró lo solicitado en esta tarea

## **Preguntas o más información**
- Las preguntas que surjan en el desarrollo de esta tarea pueden registrarlas en el slack del curso
- Recuerde que tiene a su disposición el tutorial de Creación y manejo de la Wiki [aquí](https://misovirtual.virtual.uniandes.edu.co/codelabs/wiki-github/index.html?index=..%2F..ETL#0)
