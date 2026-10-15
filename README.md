# Cursos · thebimcowork.cl/cursos

Páginas de venta de los cursos de The BIM Co-Work. Cada curso vive en su carpeta
y queda publicado en `https://thebimcowork.cl/cursos/<carpeta>/`.

| Carpeta | Curso |
|---|---|
| `gestion-bim-claude/` | Gestión BIM con Claude · 5 semanas · desde el lunes 23 de noviembre de 2026 · USD 150 |

## Publicación

Hostinger despliega este repositorio en `public_html/cursos` (hPanel → Avanzado → Git).
Cada cambio que entra a `main` se publica con el despliegue automático de Hostinger.

El directorio de despliegue tiene que ser `public_html/cursos`, nunca `public_html`: Hostinger
reemplaza los archivos del directorio en cada despliegue. Por eso la raíz de este repositorio no
lleva `index.html` ni `.htaccess`, que pisarían los del sitio si se desplegara en la raíz por error.

## Miniatura en la Academia

Las tarjetas de `/academia/` salen de los cursos del campus (`campus.thebimcowork.cl/a/cursos`),
no de este repositorio. Cada curso trae su miniatura en `img/miniatura.jpg` (1200 × 618, la
proporción de las tarjetas de la Academia) para cargarla al crear el curso en el campus:

- `gestion-bim-claude/img/miniatura.jpg` → `https://thebimcowork.cl/cursos/gestion-bim-claude/img/miniatura.jpg`
