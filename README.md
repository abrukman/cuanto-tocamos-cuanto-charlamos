# ¿Cuánto tocamos? ¿Cuánto charlamos? | Barbacoaj 2026

Estudio de los ensayos de Barbacoaj transmitidos durante 2026. Incluye el prólogo de Ariel Brukman, las estimaciones de actividad musical, el jueves promedio, mapas de calor, metodología y autoría.

## Archivos públicos

- `index.html`: informe interactivo autocontenido. No requiere compilación ni dependencias JavaScript externas.
- `informe.pdf`: versión de lectura e impresión de 15 páginas.
- `.nojekyll`: publica los archivos directamente con GitHub Pages.

## Configuración del repositorio

Repositorio propuesto: `abrukman/cuanto-tocamos-cuanto-charlamos` (público).

1. Crear un repositorio público con ese nombre, sin generar `README` ni otros archivos automáticamente.
2. Subir los tres archivos de este directorio (`index.html`, `informe.pdf` y `.nojekyll`) a la rama `main`. El `README.md` también puede subirse.
3. En **Settings > Pages**, elegir **Deploy from a branch**, rama **main**, carpeta **/(root)**, y guardar.
4. Verificar que tanto la página como el PDF funcionen en la URL publicada por GitHub Pages. La URL esperable, si no hay redirecciones heredadas, es `https://abrukman.github.io/cuanto-tocamos-cuanto-charlamos/`.

### Conectar la ruta barbacoaj.ar/cuanto-tocamos-cuanto-charlamos/

Para mantener `barbacoaj.ar` visible en la barra de direcciones y no alterar el sitio principal, se puede utilizar un **Cloudflare Worker** limitado a esa ruta. En `cloudflare/worker.js` está el código propuesto. Cambiar `ORIGIN` por la URL efectiva de GitHub Pages una vez comprobada.

1. Cloudflare > **Workers & Pages** > crear Worker e incorporar el código de `cloudflare/worker.js`.
2. Configurar una **Route**, por ejemplo `barbacoaj.ar/cuanto-tocamos-cuanto-charlamos*`, para asignar solamente esa ruta al Worker.
3. Comprobar que `https://barbacoaj.ar/cuanto-tocamos-cuanto-charlamos/` muestra el informe y que el botón **Descargar informe PDF** funciona.
4. Comprobar que `https://barbacoaj.ar/` y la ruta del sorteo siguen funcionando igual.

> **Atención:** un **Redirect Rule** simple también puede llevar al informe, pero cambia la URL visible del navegador. El Worker propuesto actúa como proxy y conserva la ruta de `barbacoaj.ar`. No añadas `CNAME` a este nuevo repositorio: el archivo `CNAME` de la web principal sigue siendo de `abrukman/barbacoaj.ar`.

No se incluye ni redistribuye el archivo de tipografía original de la banda.

## Estado metodológico

Las cifras son estimaciones acústicas automatizadas; la clasificación se calibró con muestras escuchadas por Ariel Brukman. El estudio documenta pérdidas de señal, saturación, variaciones de grabación y límites de precisión. El informe no constituye una evaluación moral de los ensayos.
