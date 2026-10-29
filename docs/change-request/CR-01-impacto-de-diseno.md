# CR-01 Programación de Pedidos Especiales: análisis de impacto desde el diseño

| Campo | Detalle |
| --- | --- |
| Change Request en Jira | SCRUM-26 |
| Rama | `feature/change-request-diseno` |
| Fase | Actividad 4. Evolución |
| Prototipo (Flujo CR) | [Ver Prototipo CR](https://www.figma.com/proto/2cQXqvXWVNV3ZQela56Ewd/ProyectoUnidad1_TastyExpress_Grupo3.?node-id=1-1376&t=LwvGiV8mPJHdgvyb-1) |

## Cambio solicitado

Permitir seleccionar una fecha y hora futura de entrega, aplicar un descuento por venta anticipada y bloquear los horarios que alcanzaron su capacidad máxima.

## Impacto en la arquitectura

- Componentes nuevos: «Servicio de Programación y Capacidad» (`/backend/programacion`) y «Programación UI» (`/frontend/programacion`).
- Interfaces nuevas: «IAgenda» (del cliente al servicio) e «ICapacidad» (el Servicio de Pedidos consulta la capacidad antes de confirmar).
- Componente modificado: Servicio de Pedidos.
- Persistencia: se guardan los horarios y su ocupación.
- Diagrama actualizado: `docs/architecture/Arquitectura_TastyExpress_v2_CR.drawio` (el diagrama original se conserva sin cambios).

## Impacto en la interfaz

Pantallas nuevas en la página «Change Request» del archivo de Figma:

- `09 Programar entrega`: selector de fecha y de hora, horarios completos deshabilitados y descuento visible en el resumen.
- `09b Horario lleno`: estado de error cuando el horario elegido alcanzó su capacidad máxima.
- `10 Pedido programado`: confirmación con fecha, hora y descuento aplicado.

Las imágenes están en `docs/design/`.

## Supuestos que deben quedar definidos en el SRS

- Descuento del 10 % sobre los productos para pedidos programados.
- Franjas horarias de 30 minutos.
- Capacidad máxima por franja: por definir.

## Requisito no funcional nuevo

Dos pedidos simultáneos no pueden superar la capacidad de una misma franja horaria.

## Pruebas nuevas y regresión

- Descuento por venta anticipada aplicado correctamente.
- Horario con capacidad máxima bloqueado.
- Fecha y hora pasadas rechazadas.
- Regresión de HU-04 (carrito) y HU-06 (confirmación del pedido).

## Artefactos actualizados

SRS, diagrama de componentes (v2), prototipo de Figma, casos de prueba y ticket SCRUM-26.
