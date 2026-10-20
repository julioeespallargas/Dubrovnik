# Ruta Ragusa

Mapa guiado de Dubrovnik para dos días: la historia de la República de Ragusa, la guerra de 1991 y los lugares de rodaje de *Juego de Tronos*. Es una sola página (`index.html`), sin dependencias ni proceso de compilación.

- **Día I · Historia:** 11 paradas por el casco antiguo.
- **Día II · Guerra y rodajes:** teleférico y monte Srđ, War Photo, escalera jesuita, Lovrijenac y, opcional, Lokrum.
- Cada parada tiene su ficha (historia, guerra, rodaje, consejo), un botón «Cómo llegar» que abre Google Maps y un marcador de visitada que se guarda en el móvil.
- Con el GPS activado, la ficha se abre sola al acercarte a unos 70 m de una parada.
- Tema claro y oscuro automático según el móvil.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `ruta-ragusa`).
2. Sube estos archivos a la raíz: `index.html`, `README.md` y `.nojekyll`.
3. En el repositorio, ve a **Settings → Pages**.
4. En **Build and deployment**, elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`. Guarda.
5. Espera uno o dos minutos. La web quedará en `https://TU-USUARIO.github.io/ruta-ragusa/`.

## Usarla en la ruta

- Ábrela desde el móvil y permite la **ubicación** cuando el navegador la pida. El GPS solo funciona en páginas con HTTPS, y GitHub Pages ya lo usa.
- Si la rechazas por error, toca el candado junto a la dirección, permite la ubicación y vuelve a tocar el indicador de GPS del mapa.
- Puedes añadirla a la pantalla de inicio desde el menú del navegador.
- Las tipografías vienen de Google Fonts, así que con poca cobertura se verá con tipos del sistema. El mapa y las fichas funcionan igual.

## Editar las paradas

Las paradas están en la lista `STOPS` dentro de `index.html`. Cada una tiene:

| Campo | Qué es |
|---|---|
| `id`, `name`, `sub` | Identificador, nombre y subtítulo |
| `day` | `1` o `2` |
| `themes` | `historia`, `guerra` y/o `got` (el primero da el color del marcador) |
| `lat`, `lon` | Coordenadas |
| `h`, `g`, `t` | Texto de historia, guerra y rodaje |
| `tip` | Consejo práctico |
| `r` | Radio de llegada en metros (opcional, 70 por defecto) |
| `opt` | `true` para una parada opcional que no entra en la línea de ruta |

## Aviso sobre los datos

- El plano es esquemático: murallas, calles y tejados son una ilustración, no un mapa a escala.
- Las coordenadas son aproximadas. Para afinarlas, en Google Maps haz clic derecho sobre el lugar y copia las coordenadas.
- Comprueba los horarios de murallas, museos, teleférico y barcos a Lokrum antes de ir, sobre todo en temporada baja.
