| **Tabla**                                   | **Campo**                                                                                                                          | **Descripcion**                                                         |
| ------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| CategoriasCliente                           | ID_Categoria                                                                                                                       | Llave primaria que identifica las categorias que puede tener un cliente |
| NombreCategoria                             | Nombre de la categoria                                                                                                             |
| Clientes                                    | ID_Cliente                                                                                                                         | Llave primaria que identifica las sucursales                            |
| Nombre                                      | Nombre del cliente                                                                                                                 |
| ClienteFactura                              | ID que identifica la sucursal princial                                                                                             |
| ID_Categoria                                | Llave foranea que hace la relación con la tabla CategoriasCliente, representa la categoria de cada cliente                         |
| ID_GrupoCompra                              | Llave foranea que hace la relación con la tabla GruposCompra, representa el grupo de compra al que pertenecen los clientes         |
| ID_CiudadEntrega                            | Llave foranea que hace la relación con la tabla Ciudad, representa la ciudad dónde se entregan los pedidos para este cliente       |
| LimiteCredito                               | Valor maximo al que este cliente puede pedir los productos bajo modalidad de credito                                               |
| FechaAperturaCuenta                         | Fecha en la que el cliente abrio cuenta con WWI                                                                                    |
| DiasPago                                    | Cantidad de días que tiene el cliente para pagar un pedido a partir de su envio                                                    |
| Ciudades                                    | ID_Ciudad                                                                                                                          | Llave primaria que identifica las ciudades                              |
| NombreCiudad                                | Nombre de la ciudad                                                                                                                |
| ID_EstadoProvincia                          | Llave foranea que hace la relación con la tabla EstadoProvincia, representa el estado o provincia en el que esta la ciudad         |
| Poblacion                                   | Numero de habitantes de la ciudad                                                                                                  |
| Colores                                     | ID_Color                                                                                                                           | Llave primaria que identifica el color                                  |
| Color                                       | Nombre del color                                                                                                                   |
| DetallesOrdenesCopia                        | Detalle_orden_ID                                                                                                                   | Llave primaria del detalle de orden                                     |
| ID_de_pedido                                | Llave foranea que hace la relación con la tabla Ordenes, representa la orden a la que el detalle esta relacionado                  |
| ID_Producto                                 | Llave foranea que hace la relacion con la tabla de Productos, representa el producto que describe el detalle de orden              |
| Descripcion                                 | Descripcion del producto                                                                                                           |
| ID_Tipo_Paquete                             | Llave foranea que hace la relacion con la tabla TipoPaquete, representa el tipo de paquete en el que se envio el producto          |
| Cantidad                                    | Cantidad de productos disponibles                                                                                                  |
| Precio_unitario                             | Valor por cada unidad del producto                                                                                                 |
| Tasa_de_impuesto                            | Valor de impuesto del producto                                                                                                     |
| Cantidad_seleccionada                       | Cantidad de productos seleccionada en la orden                                                                                     |
| Seleccion_completada_cuando                 | Fecha en la que se hizo la selección del producto                                                                                  |
| EstadosProvincias                           | ID_EstadosProvincias                                                                                                               | Llave primaria que identifica los estados y provincias                  |
| CodigoEstadoProvincia                       | Código abreviado del estado y/o provincia                                                                                          |
| NombreEstadoProvincia                       | Nombre del estado y/o provincia                                                                                                    |
| ID_pais                                     | Llave foranea que hace la relación con la tabla Paises, representa el pais en el que se encuentra el estado y/o provincia          |
| TerritorioVentas                            | Nombre del territorio en el que se encuentra el estado y/o provincia                                                               |
| Poblacion                                   | Numero de habitantes del estado y/o provincia                                                                                      |
| GruposCompra                                | ID_GrupoCompra                                                                                                                     | Llave primaria que identifica al grupo de compra                        |
| NombreGrupoCompra                           | Nombre del grupo de compra                                                                                                         |
| OrdenesCopia                                | ID_de_pedido                                                                                                                       | Llave primaria que identifica las ordenes                               |
| ID_de_cliente                               | Llave foranea que identifica al cliente que realizo la orden                                                                       |
| ID_de_vendedor                              | Llave foranea que identifica al empleado que realizo la venta                                                                      |
| Seleccionado_por_ID_de_persona              | Llave foranea que hace una relación adicional con la tabla Cliente, representa al cliente que hizo la seleccion de productos       |
| ID_de_persona_de_contacto                   | Llave foranea que hace una relacion adicional con la tabla Cliente, representa la persona de contacto de este pedido               |
| ID_de_pedido_pendiente                      |                                                                                                                                    |
| Fecha_de_pedido                             | Fecha en la que se realizo la orden                                                                                                |
| Fecha_de_entrega_esperada                   | Fecha esperada de entrega de la orden                                                                                              |
| Numero_de_pedido_de_compra_del_cliente      | Contador que lelva el conteno de las compras de cada cliente                                                                       |
| Pedido_pendiente_de_suministro_insuficiente | Valor booleano que indica si un pedido esta pendiente por falta en inventario                                                      |
| Comentarios                                 | Comentarios de la orden                                                                                                            |
| Instrucciones_de_entrega                    | Instrucciones de entrega de la orden                                                                                               |
| Comentarios_internos                        | Comentarios internos, por ejemplo de logistica                                                                                     |
| Seleccion_completada_cuando                 | Fecha en la que se seleccionaron los productos                                                                                     |
| Paises                                      | ID_pais                                                                                                                            | Llave primaria que identifica los paises                                |
| Nombre                                      | Nombre del pais                                                                                                                    |
| CodigoIsoAlpha3                             | Codigo ISO alfabetico del pais                                                                                                     |
| CodigoNumericoIso                           | codigo ISO numerico del pais                                                                                                       |
| Poblacion                                   | Numero de habitantes del pais                                                                                                      |
| Continente                                  | Nombre del continente en el que se encuentra el pais                                                                               |
| Region                                      | Region en la que se encuentra el pais                                                                                              |
| Subregion                                   | Subregion en la que se encuentra el pais                                                                                           |
| Paquetes                                    | ID_TipoPaquete                                                                                                                     | Llave primaria que identifica los tipos de paquetes                     |
| TipoPaquete                                 | Nombre del tipo de paquete                                                                                                         |
| Personas                                    | ID_persona                                                                                                                         | Llave primaria que identifica a las personas                            |
| NombreCompleto                              | Nombre de la persona                                                                                                               |
| NombreFavorito                              | Nombre preferido                                                                                                                   |
| EsEmpleado                                  | Identificador de personas que son o no empleadas                                                                                   |
| EsVendedor                                  | Identificador de personas que son o no vendedores                                                                                  |
| Producto                                    | ID_Producto                                                                                                                        | Llave primaria que identifica los productos                             |
| NombreProducto                              | Nombre de los productos                                                                                                            |
| Marca                                       | Marca del producto                                                                                                                 |
| ID_Color                                    | Llave foranea que hace la relacion con la tabla Color, representa el color principal del producto                                  |
| Necesita_refrigeracion                      | Indicador de si el producto necesita o no refrigeracion                                                                            |
| Dias_tiempo_entrega                         | Número de días máximo de entrega una vez comprado el producto                                                                      |
| Impuesto                                    | Tasa de impuesto del producto                                                                                                      |
| PrecioUnitario                              | Precio del producto por unidad                                                                                                     |
| PrecioRecomendado                           | Precio recomendado de venta al publico por unidad del producto                                                                     |
| proveedoresCopia                            | ProveedorID                                                                                                                        | Llave primaria que identifica a los proveedores                         |
| NombreProveedor                             | Nombre del proveedor                                                                                                               |
| CategoriaProveedorID                        | Llave foranea que hace la relación con la tabla CategoriaProveedor, representa la categoria de cada proveedor                      |
| PersonaContactoPrincipalID                  | Llave foranea que hace una relación con la tabla Personas, representa el contacto principal con este proveedor para WWI            |
| PersonaContactoAlternoID                    | Llave foranea que hace una relación con la tabla Personas, representa el contacto secundario con este proveedor para WWI           |
| MetodoEntregaID                             | Identificador que representa el método de entrega que usa este proveedor                                                           |
| CiudadEntregaID                             | Llave Foranea que hace la relación con la tabla Ciudad, representa la ciudad de entrega del proveedor                              |
| CiudadID                                    | Llave Foranea que hace la relación con la tabla Ciudad, representa la ciudad dónde se encuentra la principal fábrica del proveedor |
| ReferenciaProveedor                         | Identificador alfanumerico de cada proveedor                                                                                       |
| NombreCuentaBanco                           | Nombre de la entidad juridica que tiene la cuenta bancaria del proveedor                                                           |
| MarcaCuentaBanco                            | Nombre del banco                                                                                                                   |
| CodigoCuentaBanco                           | Código de la cuenta bancaria del proveedor                                                                                         |
| NumeroCuentaBaco                            | Número de la cuenta bancaria del proveedor                                                                                         |
| CodigoInternacionalBanco                    | Código SWIFT del banco                                                                                                             |
| DiasPago                                    | Cantidad de días que tiene WWI para pagar un pedido a partir de su llegada                                                         |
| ComentariosInternos                         | Comentarios internos sobre preferncias o tratos con el proveedor                                                                   |
| NumeroTelefono                              | Numero de telefono del proveedor                                                                                                   |
| NumeroFax                                   | Numero de fax del proveedor                                                                                                        |
| URL                                         | Url de la pagina web del proveedor                                                                                                 |
| Direccion1                                  | Direccion especifica del proveedor, ej. piso, numero apartamento                                                                   |
| Direccion2                                  | Direccion general del proveedor (nombre de la calle, numero)                                                                       |
| CodigoPostalEntrega                         | Codigo postal del proveedor                                                                                                        |
| UbicacionEntrega                            | Ubicación del proveedor en formato geografico                                                                                      |
| DireccionPostal1                            | Numero de caja de correo                                                                                                           |
| DireccionPostal2                            | Nombre de barrio y/o suburbio del proveedor                                                                                        |
| CodigoPostal                                | Codigo postal del proveedor                                                                                                        |
| UltimaEdicionPor                            | ID de la ultima persona del sistema que edito el registro                                                                          |
| TiposTransaccion                            | TipoTransaccionID                                                                                                                  | Llave primaria que identifica los tipos de transaccion                  |
| TipoTransaccionNombre                       | Nombre del tipo de transaccion                                                                                                     |
| MovimientosCopia                            | TransaccionProductoID                                                                                                              | Llave primaria que identifica                                           |
| ProductoID                                  | Llave foranea que hace la relación con la tabla producto, representa el producto que fue extraido o agregado en el inventario      |
| TipoTransaccionID                           | Llave foranea que hace la relación con la tabla TipoTransaccion, representa el tipo de transaccion del movimiento                  |
| ClienteID                                   | Llave foranea que hace la relación con la tabla Cliente, representa el cliente que hace la compra                                  |
| InvoiceID                                   | Identificador de la factura                                                                                                        |
| ProveedorID                                 | Llave foranea que hace la relación con la tabla Proveedor, representa el proveedor del producto en movimiento                      |
| OrdenDeCompraID                             | Llave foranea que hace la relación con la tabla de Ordenes, representa el id de la orden de este movimiento                        |
| FechaTransaccion                            | Fecha del movimiento en inventario                                                                                                 |
| Cantidad                                    | Cantidad de productos que se retiraron/ingresaron a inventario                                                                     |
| CategoriasProovedor                         | CategoriaProveedorID                                                                                                               | Llave primaria que identifica la categoria del proveedor                |
| CategoriaProveedor                          | Nombre de la categoria                                                                                                             |