# Biblioteca escolar

Catálogo de libros con buscador público. Funciona con GitHub Pages: es gratis, no necesita servidor y cualquier persona puede buscar sin crear cuenta.

## Cómo funciona

- `index.html` es la página que ve el público (buscador y filtros).
- `libros.csv` es el catálogo. **Es el único archivo que hay que editar** para agregar libros, cambiar datos o registrar préstamos.

Columnas de `libros.csv`:

| Columna | Qué poner |
|---|---|
| isbn | Opcional |
| titulo | Título del libro |
| autor | Autor |
| anio | Año de publicación |
| categoria | Ej.: Novela, Poesía, Ciencias |
| signatura | Código del estante, ej. 7A |
| copias | Cuántos ejemplares hay |
| prestados | Cuántos ejemplares están prestados ahora |

Para prestar un libro, sube el número de `prestados`. Al devolverlo, bájalo. La página muestra "Disponible" cuando `prestados` es 0 y "Prestado" cuando es igual a `copias`.

## Publicarlo (una sola vez)

1. Crea una cuenta gratis en github.com.
2. Crea un repositorio nuevo, por ejemplo `biblioteca`, y déjalo **público**.
3. Sube estos tres archivos: `index.html`, `libros.csv` y `README.md` (botón "Add file" → "Upload files").
4. Ve a **Settings → Pages**. En "Branch" elige `main` y la carpeta `/ (root)`, y guarda.
5. Espera uno o dos minutos. GitHub te mostrará la dirección pública, parecida a `https://TU-USUARIO.github.io/biblioteca/`. Ese es el enlace que compartes.

## Editar el catálogo

- **Desde GitHub:** entra al repositorio, abre `libros.csv`, pulsa el lápiz, edita y pulsa "Commit changes". En uno o dos minutos la página pública se actualiza.
- **Desde Excel o Google Sheets:** edita el archivo ahí, expórtalo como CSV y súbelo reemplazando `libros.csv`. La página entiende CSV separados por coma o por punto y coma, y con tildes.

## Quién puede qué

- **Público:** solo ve la página y busca. No puede cambiar nada.
- **Encargada:** en el repositorio, ve a **Settings → Collaborators** y agrega su usuario de GitHub (ella necesita su propia cuenta gratis). Así puede editar `libros.csv` sin tener acceso a nada más.
- **Tú:** eres el dueño del repositorio y mantienes todos los permisos.

## Ojo

El repositorio es público, así que `libros.csv` también lo es. No pongas ahí nombres de alumnos que tienen libros prestados; solo la cantidad de ejemplares prestados.
