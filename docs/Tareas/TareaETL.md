# Tarea: ETL

# Introducción

**Objetivo**

Realizar un proceso ETL básico en Pyspark

**¿Para qué?**

Practicar lo aprendido en el tutorial de ETL

**¿Qué necesita?**

1. Modelo multidimensional asociado al proceso de movimientos
2. Notebook para trabajar: puede usar la seccion 3 "Espacio para desarrollar la tarea" al final del notebook del tutorial para realizar esta actividad
5. Servidor SQL con base de datos relacional "WWImportersTransactional" y base de datos relacional que corresponde a la bodega de WWI de cada estudiante "Estudiante_i"

# Enunciado
Ahora que sabe cómo realizar un proceso ETL, dado el modelo multidimensional del proceso de negocio de movimientos de inventario realice las siguientes actividades:
1. **Entregable 1 - Diseño del ETL:** Diseñe el ETL para las dimensiones proveedor, tipoTransaccion, fecha y para la tabla de hechos. A nivel de la tabla de proveedores incluya la tabla categoriasProveedores donde encuentra información de las categorías. El diseño del ETL es un diagrama como lo encuentra en la infografía de proceso ETL y puede observar en la siguiente figura. En el entregable utilice la siguiente [plantilla para presentar el diseño de ETL](PlantillaDiseñoETL.xlsx) e incluya una descripción general que permita comprender detalles que pueden ser confusos.  
![Diseño ETL tabla empleados](Img/DiseñoETL.PNG)

3. **Entregable 2 - Implementación del ETL:** implementación del proceso ETL para las dimensiones Proveedor, TipoTransaccion, Fecha y para la tabla de hechos. En el entregable incluya una descripción general que permita comprender el proceso de implementación del ETL.

Note que para este proceso de negocio, las dimensiones Producto y Cliente son iguales a las del hecho Orden, este caso se conoce como dimensiones compartidas. Usted debe concentrarse en las dimensiones Proveedor, TipoTransaccion, Fecha y la tabla de hechos que no existen en la bodega de datos actualmente.

WWImporters le comenta que el módelo dimensional estará disponible después de la entrega de la tarea de modelado de datos.

WWImporters tambien le comenta que Las respuestas del negocio estarán disponibles después de la entrega de la tarea de entendimiento de datos

Los datos revisados por el negocio quedan en las tablas Proveedores y movimientos y estos son los que deben utilizar en el proceso ETL. Por otra parte, en las tablas ProveedoresCopia y movimientosCopia quedan los datos con errores en caso de que deseen revisar/ejecutar el ejercicio que realizó de entendimiento de datos.

# Recuerde
- El diseño es fundamental y en particular el detalle de las transformaciones
- Dejar evidencia de las tablas creadas y pobladas en la base de datos que le fue asignada en el curso
- Entregar el notebook únicamente con la información solicitada en la tarea
