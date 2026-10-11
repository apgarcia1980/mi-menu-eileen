# Mi Menú · Eileen

Aplicación móvil de menú y lista de compra basada en el documento nutricional del 10/10/2026. Cero dependencias: HTML, CSS, JavaScript y PWA.

## Desplegar en Vercel

1. Descomprime este ZIP y sube la carpeta a un repositorio de GitHub (archivos en la raíz del proyecto).
2. En Vercel: **Add New → Project → Import Git Repository**.
3. Framework preset: **Other**. Build command: **vacío**. Output directory: **vacío o `.`** (raíz del proyecto).
4. **Deploy**. Abre la URL HTTPS de Vercel en el iPhone; Safari → Compartir → Añadir a pantalla de inicio.

También puedes instalar Vercel CLI (`npm i -g vercel`), entrar a la carpeta del proyecto y ejecutar `vercel --prod`.

## Funciona sin backend

- Menús y cambios guardados en `localStorage` del propio navegador.
- La lista de compra se genera desde las opciones elegidas y conserva las marcas de cada semana.
- Copia de datos exportable desde la sección Compra en formato JSON (restaurable desde el botón «Recuperar copia»).
- Sin registro, sin sincronización entre dispositivos.
- Los domingos están marcados como pendientes, ya que no constan en el documento.
- Las meriendas de entrenamiento indicadas en el documento están disponibles los lunes. Si la nutricionista confirma su aplicación en otros días, se puede ampliar.
- Algunas recetas del documento no incluyen pesos: no se inventan. Las alternativas separadas por «O» no se suman; la compra muestra las opciones y requiere que la persona elija qué producto llevar.
- Las ilustraciones de comida son iconos, no fotografías: se ha priorizado entregar una versión funcional ligera hoy mismo.

## Prueba local

Ejecuta `python -m http.server 8080` dentro de la carpeta y abre `http://localhost:8080`.

## Notas

Esta aplicación organiza el contenido del plan, no lo sustituye ni genera nuevas recomendaciones nutricionales. El menú base sigue el orden semanal indicado. La planificación puede consultarse semana a semana avanzando o retrocediendo con las flechas.
