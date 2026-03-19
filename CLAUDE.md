# CLAUDE.md — TPC Daniel Del Toro Calendar

## Qué es esto
Página web estática alojada en Cloudflare Pages que muestra el calendario de contenido del proyecto Daniel Del Toro. Se actualiza automáticamente cada vez que se pushea a GitHub.

- **Repo GitHub:** https://github.com/Daniel-Figutech/tpc-daniel-deltoro
- **URL en producción:** (pegar aquí el link de Cloudflare Pages cuando esté listo)
- **Calendario Google:** TPC Daniel Del Toro — ID: `39ee63d5fdce8964a87c2dcb560e9040034c7ea40d44bfe53db3ca3f00e1605b@group.calendar.google.com`

## Cómo desplegar cambios
```bash
git add .
git commit -m "descripción del cambio"
git push
```
Cloudflare Pages detecta el push y redespliega automáticamente en ~30 segundos.

## Estructura del proyecto
```
tpc-daniel-deltoro/
└── index.html    ← toda la página (HTML + CSS inline)
```

## Qué puedes pedirme que cambie
- **Diseño:** colores, tipografía, layout, modo claro/oscuro
- **Vista del calendario:** semana / mes / agenda — cambiar el parámetro `mode=WEEK` en el iframe por `MONTH` o `AGENDA`
- **Idioma:** cambiar `hl=es` por otro código de idioma
- **Branding:** nombre, colores del punto, badge, leyenda de eventos
- **Añadir secciones:** descripción del proyecto, links, contacto del equipo

## Parámetros del embed de Google Calendar (en el iframe src)
| Parámetro | Valor actual | Opciones |
|-----------|-------------|----------|
| `mode` | `WEEK` | `WEEK`, `MONTH`, `AGENDA` |
| `hl` | `es` | `es`, `en`, `fr`... |
| `showNav` | `1` | `0` oculta navegación |
| `showTabs` | `1` | `0` oculta pestañas semana/mes/agenda |
| `showTitle` | `0` | `1` muestra título del calendario |

## Nota importante
El calendario de Google debe estar en **público** para que el embed funcione para usuarios externos. Si deja de verse, verificar en Google Calendar → Configuración → TPC Daniel Del Toro → "Hacer público este calendario".
