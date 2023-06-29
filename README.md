# Proyectosistemas
Se hace la creacion de la base de dato para la farmacia belay despues se crea la tabla tomando los datos del codigo, nombre, minimo stock, el stock recomendado, el precio que tiene y por ultimo se toma el stock que tiene, la clave sera el codigo del producto.

*create database farmaciabeley*
*use farmaciabeley*
*create table farmbeley (codigo int(50), nombre varchar(100), minimo int, recomendado int, precio int, stock int,primary key (codigo))*

Despues se crea la tabla de bioequivalentes para tener en cuenta los medicamentos que son bioequivalentes entre si, se toman los datos del codigo unificador que se crea, con el codigo original y el nombre del producto , la clave sera el codigo unificador.

*create table bioequivalente (codunificador varchar(50), codigo varchar(50), nombre varchar(50),primary key (codunificador));*

Se hace la creacion de la base de dato para los precios de los proveedores y su existecia, se crean las tablas para los distintos proveedores donde se toma el codigo interno que se tiene en los proovedores, el codigo de barra, la descripcion del articulo, el nombre que este tiene, su principal activo, el precio de venta y el stock que este tiene. El codigo interno sera nuestra clave.

*create database precio_proovedor*
*use precio_proovedor*
*create table clininmarket1 (codigo_int(50), ean varchar(50), descripcion_ art varchar(200), nombre_pro varchar(200),principio_act varchar(200), precio_venta int, stock int, primary key (codigo))*
*create table clininmarket2 (codigo_int(50), ean varchar(50), descripcion_ art varchar(200), nombre_pro varchar(200),principio_act varchar(200), precio_venta int, stock int, primary key (codigo))* 
*create table clininmarket3 (codigo_int(50), ean varchar(50), descripcion_ art varchar(200), nombre_pro varchar(200),principio_act varchar(200), precio_venta int, stock int, primary key (codigo))*
*create table clininmarket4 (codigo_int(50), ean varchar(50), descripcion_ art varchar(200), nombre_pro varchar(200),principio_act varchar(200), precio_venta int, stock int, primary key (codigo))*
*create table farmaciascarebean1 (codigo int(50), ean varchar(50), descripcion_art varchar(200), nombre_pro varchar(200),principio_ act varchar(200), precio_ venta int, stock int, primary key (codigo))*
*create table farmaciascarebean2 (codigo int(50), ean varchar(50), descripcion_art varchar(200), nombre_pro varchar(200),principio_ act varchar(200), precio_ venta int, stock int, primary key (codigo))*
*create table farmaciascarebean3 (codigo int(50), ean varchar(50), descripcion_art varchar(200), nombre_pro varchar(200),principio_ act varchar(200), precio_ venta int, stock int, primary key (codigo))*

Se crean tres tablas para poder obtener la informacion de los proveedores (tabla contiene el rut del proveedor, el nombre y su direccion) y por otra parte se crea la tabla para la traduccion de los distintos productos donde esta tabla de los porductos de los proveedores tiene el codigounifica del proveedor, nuestro codigo unifificador, el rut del proveedor, el nombre del producto, la descripcion dde este  , el stock que iene y el recomendado y por ultimo su costo unitario donde codigo producto es nuestra clave.
por ultimo se hace la tabla de mismo producto  donde se llena con el codigo unificador , el nombre, la descripcion y el codigo del proveedor y la clave sera el codigo unificador


*create table mismo_producto (codunificadorpr varchar(50) not null, nombre varchar(50), descripcion text,
codigo de _proveedor int(3), costo unitario int(10), foreign key (codunificadorpr));*
*create table proovedor(Rut_proveedor varchar(20) not null, nombre_proveedor varchar(50),direccion text
primary key (Rut_proveedor));*
*create table producto_proovedor(codproducto varchar(50), codunificadorpr varchar(50), proveedor_rut varchar(20),
nombre varchar(50), descripcion text, stock int(3), stock_recomendado int(3), costo_unitario int(10), primary key
(codproducto), foreign key (codunificadorpr), foreign key (proveedor_rut));*

Todos los datos que se obtienen es a travez de la importancian de tablas de excel tanto de la farmacia beley como de los proveedores 

