# ProyectoUnidad1_TastyExpress_Grupo3

**TastyExpress: Sistema de Gestión de Pedidos y Delivery para Restaurantes**

Proyecto de la Unidad 1 de Ingeniería de Software. Recorre las cuatro fases del ciclo de vida del software (especificación, diseño e implementación, validación y evolución) con herramientas en sus versiones gratuitas.

## Integrantes

Grupo 3: Mateo Aymacaña, Mateo Cevallos, Bryan Gudiño y Danny Sivinta.

Docente: Dra. Eleana Jerez Villota.

## Caso asignado

**TastyExpress**: plataforma web para restaurantes de comida rápida y entregas a domicilio.

- **Alcance base:** catálogo digital de menú, consulta de productos y precios, personalización de ingredientes, carrito de compras, registro de dirección, confirmación del pedido, seguimiento del estado del pedido y del repartidor en un mapa, y facturación.
- **Change Request (Actividad 4):** «Programación de Pedidos Especiales». Permite seleccionar una fecha y hora futura de entrega, aplicar un descuento por venta anticipada y bloquear los horarios que alcanzaron su capacidad máxima.

## Enlaces del proyecto

* **Jira (Backlog, TEST, Bugs y Change Request):** [ProyectoUnidad1_TastyExpress_Grupo3](https://tasty-express-grupo3.atlassian.net/jira/software/projects/SCRUM/boards/1)
* **Confluence (SRS y documentación):** [SRS TastyExpress](https://tasty-express-grupo3.atlassian.net/wiki/spaces/P/pages/66049/Especificaci+n+de+Requisitos+de+Software+SRS+-+TastyExpress)
* **Diseño en Figma:** [Archivo de Figma](https://www.figma.com/design/2cQXqvXWVNV3ZQela56Ewd/ProyectoUnidad1_TastyExpress_Grupo3.?node-id=0-1&t=qGx0njza8hsoha9r-1)
* **Prototipo interactivo, Flujo 1 (Explorar y armar pedido):** [Ver prototipo](https://www.figma.com/proto/2cQXqvXWVNV3ZQela56Ewd/ProyectoUnidad1_TastyExpress_Grupo3.?t=qGx0njza8hsoha9r-1)
* **Prototipo interactivo, Flujo 2 (Checkout y seguimiento):** [Ver prototipo](https://www.figma.com/proto/2cQXqvXWVNV3ZQela56Ewd/ProyectoUnidad1_TastyExpress_Grupo3.?node-id=1-1375&t=qGx0njza8hsoha9r-1)
* **Prototipo interactivo, Flujo CR (Programar pedido):** [Ver prototipo](https://www.figma.com/proto/2cQXqvXWVNV3ZQela56Ewd/ProyectoUnidad1_TastyExpress_Grupo3.?node-id=1-1376&t=LwvGiV8mPJHdgvyb-1)
* **Diagrama de componentes (editable y exportado):** [docs/architecture](docs/architecture)

## Estructura del repositorio

```
/
├── backend/             Código del backend
├── frontend/            Código del cliente web
└── docs/
    ├── architecture/    Diagrama de componentes: v1 y v2 con el Change Request (.drawio y .png)
    ├── bugs/            Registro de los defectos corregidos
    ├── change-request/  Análisis de impacto del CR-01 desde el diseño
    └── design/          Evidencias de diseño (pantallas del prototipo)
```

## Instrucciones de ejecución

<!-- C: confirmar estos comandos con la tecnología real del proyecto antes de entregar. -->

Requisitos: Node.js y npm.

Frontend:

```
cd frontend
npm install
npm run dev
```

Backend:

```
cd backend
npm install
npm start
```

Cada carpeta puede incluir su propio README con detalles adicionales.

## Flujo de trabajo

El trabajo se realiza en ramas y se integra a `main` mediante Pull Request con revisión de otro integrante:

- `feature/[nombre-corto]` para funcionalidades y documentación.
- `fix/[nombre-corto]` para corrección de defectos.

| Pull Request | Contenido |
| --- | --- |
| [#1](https://github.com/cevallosmateo07-byte/ProyectoUnidad1_TastyExpress_Grupo3/pull/1) | Diagrama de componentes (Actividad 2) |
| [#3](https://github.com/cevallosmateo07-byte/ProyectoUnidad1_TastyExpress_Grupo3/pull/3) | Corrección del filtro de precio, Bug SCRUM-35 (Actividad 3) |
| [#5](https://github.com/cevallosmateo07-byte/ProyectoUnidad1_TastyExpress_Grupo3/pull/5) | Diseño y arquitectura del Change Request CR-01 (Actividad 4) |

## Trazabilidad en Jira

| Elemento | Claves |
| --- | --- |
| Historias de usuario | SCRUM-17 a SCRUM-24 (HU-01 a HU-08) |
| Casos de prueba | SCRUM-27 a SCRUM-34 (TEST-01 a TEST-08) |
| Bug corregido | SCRUM-35 (vinculado a TEST-02 y a HU-02) |
| Requisitos no funcionales | SCRUM-39 a SCRUM-42 (RNF-01 a RNF-04) |
| Change Request | SCRUM-26 (CR-01) |

## Herramientas

Jira, Confluence, draw.io, Figma y GitHub, todas en sus versiones gratuitas.
