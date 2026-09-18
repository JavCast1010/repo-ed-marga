# Proyecto de productos

Proyecto inicial para gestionar productos y preparar una interfaz de acceso de usuarios.

## Estructura

```text
.
├── backend/
│   └── productos.sql
└── frontend/
    ├── login.html
    ├── registroU.html
    └── style.css
```

## Base de datos

La tabla `productos` almacena:

- `id`: identificador unico autoincremental.
- `nombre`: nombre del producto.
- `descripcion`: informacion adicional del producto.
- `precio`: precio con dos decimales.
- `stock`: cantidad disponible.
- `categoria`: categoria del producto.
- `imagen_url`: URL de la imagen del producto.
- `creado_en`: fecha de creacion.
- `actualizado_en`: fecha de la ultima actualizacion.

### Instalacion

1. Abre MySQL o MariaDB.
2. Crea o selecciona una base de datos:

```sql
CREATE DATABASE tienda;
USE tienda;
```

3. Ejecuta el archivo `backend/productos.sql`.

Desde la terminal tambien puedes ejecutar:

```bash
mysql -u usuario -p tienda < backend/productos.sql
```

Cambia `usuario` por tu usuario de MySQL.

## Frontend

Para probar la interfaz, abre `frontend/login.html` directamente en el navegador. Actualmente contiene la plantilla inicial de la pantalla de login; las pantallas de registro y los estilos estan preparadas para desarrollarse.

## Estado actual

- Tabla SQL de productos creada.
- Plantilla inicial de login creada.
- Formulario de registro pendiente.
- Conexion entre frontend y backend pendiente.
- Operaciones para crear, consultar, actualizar y eliminar productos pendientes.

## Tecnologias

- HTML5
- CSS3
- MySQL o MariaDB
