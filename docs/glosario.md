---
hide:
  - footer
---

Definiciones de términos comunes usados en la APIs de Tecopos

## **<bold id="areas">Áreas</bold>**

Las áreas pueden ser considerados como departamentos dentro de un negocio.

### Tipos de áreas

- Área de procesado (MANUFACTURER)
- Almacenes (STOCK)
- Tienda Online (SALE)
- Punto de acceso (ACCESSPOINT)


## **Productos**

Los productos constituyen bienes de un negocio. Estos bienes poseen características comunes: nombre, descripción, código de barra, cantidad, etc. Según el propósito de su obtención y la utilidad que ofrezcan pueden ser clasificados.

### <bold id="tipos-productos">Tipos de productos</bold>

| **Listos para vender** | **Almacenables** |
| ---- | ---- |
| Elaborado | Materia prima |
| Almacén | Procesado |
| Variable | Desperdicio |
| Servicio | Activo fijo |
| Agrego |  |
| Combo |  |

### Operaciones sobre productos

A continuación se definen las operaciones que registran un cambio en el estado de los productos:

- _Entrada_: Recepción de un producto en el almacén después de un proceso de compra.
    
- _Traslado:_ Movimiento de uno o más productos de un almacén a otro.
    
- _Salida:_ Baja de un producto del inventario por concepto definido por el usuario.
    
- _Ajuste:_ Conciliación del inventario.
    
- _Transformación:_ Conversión de un producto en otro.
    
- _Venta:_ Baja de un producto del inventario por concepto de venta.
	
- *Merma*: Disminución de un producto por desperdicio.

## **Clientes**

Los clientes forman parte de los principales destinos de un producto como venta.

## **Proveedores**

Los proveedores son las entidades y/o organismos que suministren productos a un negocio.

## **Usuarios**

Los usuarios son las personas que hacen uso de la API de Tecopos mediante aplicaciones clientes ya sean móviles o web. Según el rol que posean es el conjunto de permisos que adquieren sobre los recursos y funcionalidades del sistema.

### <bold id="roles">Roles de usuarios</bold>

Seguidamente se mencionan los roles existentes y casos de uso ordenados de mayor en menor medida de nivel de permisos:

| Rol | Casos de uso |
| ---- | ---- |
| Administrador | Propietario del negocio |
| Control | Contabilidad, Jefe de almacén, Manejador de ciclos económicos, Operario de producción  |
| Público | Operadores (tienda online, punto de venta, punto de acceso), Camarero |
