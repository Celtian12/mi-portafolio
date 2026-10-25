# Tienda TECSUP

![Banner de Tienda TECSUP](https://placehold.co/600x150/0072ce/ffffff.png?text=Tienda+TECSUP)

Proyecto de práctica para el **Laboratorio 03** del curso Diseño de Interfaces de Programación Avanzado en [TECSUP](https://www.tecsup.edu.pe).

Para obtener más detalles sobre el flujo de trabajo y cómo reportar errores mediante Issues o Pull Requests, revisa nuestra [Guía de Contribución](docs/GUIA.md).

## Características y Estructura

Este proyecto muestra un resumen de compra aplicando tecnologías web básicas:

- Estructura semántica de productos en tabla HTML.
- Diseño limpio utilizando los colores institucionales del curso.
- Cálculo dinámico del monto total a pagar (S/ 68.00).

### Archivos del Proyecto

A continuación se describen los archivos principales que componen el repositorio:

| Archivo       | Tipo | Descripción                                                               |
| :------------ | :--- | :------------------------------------------------------------------------ |
| `index.html`  | HTML | Estructura principal con la tabla de productos y el contenedor del total. |
| `estilos.css` | CSS  | Estilos visuales, bordes de tabla y formato de texto.                     |
| `script.js`   | JS   | Lógica de programación para calcular y renderizar el total de la compra.  |

## Instalación y Uso

Sigue estos pasos numerados para probar el proyecto localmente:

1. Abre tu terminal y clona el repositorio ejecutando el comando `git clone <url-del-repositorio>`.
2. Ingresa a la carpeta del proyecto descargado.
3. Abre el archivo `index.html` en tu navegador web de preferencia.

### Lógica de Cálculo

El archivo `script.js` se encarga de procesar la lista de productos mediante la siguiente función:

```javascript
function calcularTotal(lista) {
  let total = 0
  for (const producto of lista) {
    total = total + producto.precio * producto.cantidad
  }
  return total
}
```

### Estado de Tareas

- [x] Crear estructura de tabla en `index.html`.
- [x] Corregir la vinculación de `estilos.css` en la rama `fix-styles`.
- [x] Implementar el cálculo automático de precios en `script.js`.
- [ ] Agregar un formulario para insertar nuevos productos dinámicamente.
