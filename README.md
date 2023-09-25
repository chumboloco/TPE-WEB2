santiagoandiarena@gmail.com blapano@gmail.com
Tienda de camisetas online
Un sitio web diseñado para la venta de camisetas online al estilo de gmkits1, entre otras.

Table Cliente {
  Cliente_ID integer [primary key]
  Nombre varchar(45)
  Apellido varchar(45)
  Domicilio varchar(45)
  Ciudad varchar(45)
}

Table Pedido {
  Pedido_ID integer [primary key]
  Cliente_ID integer
  Producto_ID integer
  Domicilio varchar(45)
  Ciudad varchar(45)
}

Table Producto {
  Producto_ID integer [primary key]
  Equipo varchar(45)
}

Ref: Cliente.Cliente_ID - Pedido.Cliente_ID

Ref: Producto.Producto_ID - Pedido.Producto_ID