# Corrección del filtro «Hasta $5.00» del catálogo

| Campo | Detalle |
| --- | --- |
| Bug en Jira | SCRUM-35 |
| TEST que falló | TEST-02 (SCRUM-28), historia HU-02 (SCRUM-18) |
| Rama | `fix/filtro-precio` |
| Fase | Actividad 3. Validación |
| Prototipo (Flujo 1) | [Prototipo Flujo 1](https://www.figma.com/proto/2cQXqvXWVNV3ZQela56Ewd/ProyectoUnidad1_TastyExpress_Grupo3.?t=qGx0njza8hsoha9r-1) |

## Defecto

Al pulsar el filtro «Hasta $5.00» en `01 Catálogo`, el prototipo no cambiaba la lista de productos y seguía mostrando los seis.

- **Resultado esperado (criterio de aceptación de HU-02):** solo los productos de $5.00 o menos: Coca-Cola 500 ml ($1.25) y Brownie ($2.50).
- **Resultado obtenido:** los seis productos, incluidos los de $5.50 a $8.50.

## Corrección

Se añadió al prototipo de Figma la pantalla `01c Catálogo filtrado`, con el filtro en estado activo y solo los productos que cumplen la condición. Se conectó:

- en `01 Catálogo`, el grupo `Filtro Hasta $5.00` lleva a `01c Catálogo filtrado`;
- en `01c Catálogo filtrado`, el grupo `Filtro Hasta $5.00 (activo)` lleva de vuelta a `01 Catálogo`.

Evidencia de la pantalla corregida: `docs/design/01c-catalogo-filtrado.png`.

## Reprueba

Pendiente: QA reejecutará el TEST-02 sobre el prototipo corregido una vez fusionado este Pull Request y registrará el resultado en Jira (SCRUM-28).
