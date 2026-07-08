# Modelo de Datos

## Objetivo

Diseñar la estructura de la base de datos para ByteCore IA.

---

# Entidades

## Empresa
Descripción (qué representa).
Campos (nombre, tipo de dato, descripción).
Relaciones (con qué otras entidades se conecta).
Reglas de negocio específicas.
...

## Usuario
Descripción (qué representa).
Campos (nombre, tipo de dato, descripción).
Relaciones (con qué otras entidades se conecta).
Reglas de negocio específicas.
...

## Producto
Descripción (qué representa).
Campos (nombre, tipo de dato, descripción).
Relaciones (con qué otras entidades se conecta).
Reglas de negocio específicas.
...

## Cliente
Descripción (qué representa).
Campos (nombre, tipo de dato, descripción).
Relaciones (con qué otras entidades se conecta).
Reglas de negocio específicas.
...

## Pedido
Descripción (qué representa).
Campos (nombre, tipo de dato, descripción).
Relaciones (con qué otras entidades se conecta).
Reglas de negocio específicas.
...

## Venta
Descripción (qué representa).
Campos (nombre, tipo de dato, descripción).
Relaciones (con qué otras entidades se conecta).
Reglas de negocio específicas.
...

## Conversacion
Descripción (qué representa).
Campos (nombre, tipo de dato, descripción).
Relaciones (con qué otras entidades se conecta).
Reglas de negocio específicas.
...

## ConfiguracionIA
Descripción (qué representa).
Campos (nombre, tipo de dato, descripción).
Relaciones (con qué otras entidades se conecta).
Reglas de negocio específica
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
