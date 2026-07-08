# Historias de Usuario

**Proyecto:** ByteCore IA Solutions  
**Versión:** 1.0  
**Autor:** Kevin Vélez  
**Fecha:** Julio 2026

---

# Introducción

Las historias de usuario describen las funcionalidades que deberá ofrecer ByteCore IA Solutions desde la perspectiva de quienes interactúan con el sistema. Estas historias servirán como base para el desarrollo de la aplicación, permitiendo organizar las funcionalidades en módulos, priorizar el trabajo y garantizar que el producto responda a las necesidades reales de los usuarios.

Las historias de usuario se encuentran agrupadas por épicas, las cuales representan los principales módulos del sistema.

---

# ÉPICA 1 - Gestión de Empresas y Autenticación

## HU-001 - Registrar empresa

**Prioridad:** Alta

**Actor:** Emprendedor

**Descripción**

Como emprendedor deseo registrar mi empresa para comenzar a utilizar ByteCore IA Solutions y administrar mi negocio desde la plataforma.

### Criterios de aceptación

- El sistema deberá solicitar el nombre de la empresa.
- El sistema deberá solicitar el NIT.
- El sistema deberá solicitar correo electrónico.
- El sistema deberá solicitar teléfono.
- El sistema deberá crear automáticamente un usuario administrador.
- El correo electrónico no podrá estar registrado previamente.

### Reglas de negocio

- El correo de la empresa debe ser único.
- El NIT debe ser único.
- Toda empresa debe tener al menos un usuario administrador.

### Dependencias

Ninguna.

### Estimación

5 Story Points

---

## HU-002 - Iniciar sesión

**Prioridad:** Alta

**Actor:** Administrador

**Descripción**

Como administrador deseo iniciar sesión para acceder al panel administrativo de mi empresa.

### Criterios de aceptación

- Validar correo electrónico.
- Validar contraseña.
- Mostrar el Dashboard después de autenticarse.
- Mostrar mensaje de error cuando las credenciales sean incorrectas.

### Reglas de negocio

- Solo usuarios activos podrán iniciar sesión.

### Dependencias

HU-001

### Estimación

3 Story Points

---

# ÉPICA 2 - Gestión de Productos

## HU-003 - Registrar producto

**Prioridad:** Alta

**Actor:** Administrador

**Descripción**

Como administrador deseo registrar productos para que puedan ser consultados por los clientes mediante el asistente virtual.

### Criterios de aceptación

- Registrar nombre.
- Registrar descripción.
- Registrar precio.
- Registrar stock.
- Asociar el producto a una categoría.
- Asociar el producto a la empresa.

### Reglas de negocio

- El precio debe ser mayor que cero.
- El stock no puede ser negativo.

### Dependencias

HU-002

### Estimación

5 Story Points

---

## HU-004 - Editar producto

**Prioridad:** Alta

**Actor:** Administrador

**Descripción**

Como administrador deseo modificar la información de un producto para mantener actualizado el catálogo.

### Criterios de aceptación

- Permitir modificar todos los datos del producto.
- Guardar los cambios realizados.

### Dependencias

HU-003

### Estimación

3 Story Points

---

## HU-005 - Desactivar producto

**Prioridad:** Media

**Actor:** Administrador

**Descripción**

Como administrador deseo desactivar un producto para evitar que continúe apareciendo en las consultas realizadas por los clientes.

### Criterios de aceptación

- El producto no debe eliminarse físicamente.
- El producto debe marcarse como inactivo.

### Dependencias

HU-003

### Estimación

2 Story Points

---

# ÉPICA 3 - Gestión de Clientes

## HU-006 - Registrar cliente

**Prioridad:** Alta

**Actor:** Administrador

**Descripción**

Como administrador deseo registrar clientes para mantener organizada la información de quienes compran en el negocio.

### Criterios de aceptación

- Registrar nombre.
- Registrar teléfono.
- Registrar correo electrónico (opcional).
- Registrar dirección.

### Dependencias

HU-002

### Estimación

3 Story Points

---

## HU-007 - Consultar clientes

**Prioridad:** Media

**Actor:** Administrador

**Descripción**

Como administrador deseo consultar el listado de clientes registrados para acceder rápidamente a su información.

### Estimación

2 Story Points

---

# ÉPICA 4 - Atención por WhatsApp

## HU-008 - Consultar productos mediante WhatsApp

**Prioridad:** Alta

**Actor:** Cliente

**Descripción**

Como cliente deseo consultar productos mediante WhatsApp para obtener información sin necesidad de comunicarme con un asesor.

### Criterios de aceptación

- El asistente deberá responder automáticamente.
- Deberá consultar la información almacenada en la base de datos.
- Deberá responder utilizando lenguaje natural.

### Dependencias

HU-003

### Estimación

8 Story Points

---

## HU-009 - Crear pedido

**Prioridad:** Alta

**Actor:** Cliente

**Descripción**

Como cliente deseo solicitar productos mediante WhatsApp para iniciar un proceso de compra.

### Criterios de aceptación

- El sistema deberá crear un pedido pendiente.
- El pedido deberá quedar asociado al cliente.
- El pedido deberá quedar asociado a la empresa.

### Reglas de negocio

- El pedido no representa una venta definitiva.

### Dependencias

HU-008

### Estimación

8 Story Points

---

# ÉPICA 5 - Gestión de Pedidos

## HU-010 - Confirmar pedido

**Prioridad:** Alta

**Actor:** Administrador

**Descripción**

Como administrador deseo confirmar un pedido para convertirlo en una venta.

### Criterios de aceptación

- Crear la venta.
- Actualizar el inventario.
- Registrar el ingreso correspondiente.

### Dependencias

HU-009

### Estimación

5 Story Points

---

## HU-011 - Cancelar pedido

**Prioridad:** Media

**Actor:** Administrador

**Descripción**

Como administrador deseo cancelar un pedido cuando el cliente decida no realizar la compra.

### Estimación

2 Story Points

---

# ÉPICA 6 - Inteligencia Artificial

## HU-012 - Configurar el asistente

**Prioridad:** Alta

**Actor:** Administrador

**Descripción**

Como administrador deseo configurar el comportamiento del asistente para personalizar la atención según las necesidades de mi negocio.

### Criterios de aceptación

- Configurar mensaje de bienvenida.
- Configurar prompt base.
- Configurar horario de atención.
- Configurar idioma.

### Estimación

5 Story Points

---

# ÉPICA 7 - Reportes

## HU-013 - Consultar ventas

**Prioridad:** Alta

**Actor:** Administrador

**Descripción**

Como administrador deseo consultar las ventas realizadas para conocer el desempeño del negocio.

### Estimación

3 Story Points

---

## HU-014 - Consultar productos más vendidos

**Prioridad:** Media

**Actor:** Administrador

**Descripción**

Como administrador deseo identificar los productos más vendidos para apoyar la toma de decisiones.

### Estimación

3 Story Points

---

## HU-015 - Registrar movimientos contables

**Prioridad:** Media

**Actor:** Administrador

**Descripción**

Como administrador deseo registrar ingresos y egresos para llevar un control financiero básico.

### Estimación

5 Story Points

---

# Conclusión

Las historias de usuario definidas constituyen la base funcional de ByteCore IA Solutions y servirán como guía para el desarrollo de cada uno de los módulos del sistema. Estas historias serán implementadas progresivamente durante los diferentes sprints del proyecto, siguiendo una metodología de desarrollo incremental.
