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

Desde el 01-10-2026 `/academia/` no consulta el campus: `academia/index.php` sirve
`academia/index.html` tal cual, porque ya no lleva las marcas `cursos:tarjetas` y `cursos:paneles`.
Cada curso se agrega a mano en ese archivo, con una tarjeta y su panel. La miniatura de cada curso
está en `img/miniatura.jpg` (1200 × 618, la proporción de las tarjetas):

- `gestion-bim-claude/img/miniatura.jpg` → `https://thebimcowork.cl/cursos/gestion-bim-claude/img/miniatura.jpg`

## Formulario de registro

La sección `#reservar` de cada curso envía a `https://thebimcowork.cl/reserva-cupo.php`. Ese
archivo vive solo en el servidor (`public_html/reserva-cupo.php` y su `reserva-cupo.config.php`),
fuera de este repositorio. Guarda cada registro en `public_html/_registros/` (sin acceso desde el
navegador) y avisa por correo a thebimcowork@gmail.com. La planilla de Google Drive «Reservas de
cupo · Gestión BIM con Claude» lee los registros con `=IMPORTDATA(...)`.

Para un curso nuevo, agrega su carpeta a `RC_CURSOS` en `reserva-cupo.php`.
