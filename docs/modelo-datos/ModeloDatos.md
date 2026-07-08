# Modelo de Datos

## Objetivo

Diseñar la estructura de la base de datos para ByteCore IA.

---

# Entidades

## Empresa

...

## Usuario

...

## Producto

...

## Cliente

...

## Pedido

...

## Venta

...

## Conversacion

...

## ConfiguracionIA

...

---

# Relaciones

Empresa 1 --- N Usuarios

Empresa 1 --- N Productos

Empresa 1 --- N Clientes

...

---

# Reglas de Negocio

- Una empresa solo puede visualizar su propia información.
- Todo pedido debe pertenecer a una empresa.
- Una venta solo puede generarse a partir de un pedido confirmado.
- El inventario se descuenta únicamente cuando la venta es confirmada.
