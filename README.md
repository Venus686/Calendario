# Calendario de otoño 2026

Calendario de octubre a diciembre de 2026 con todo lo que hay que seguir, en **hora de España peninsular**:

- **Mundial de LoL** (15 oct – 14 nov): Play-In, fase suiza, cuartos, semifinales y final.
- **UEFA Nations League**: solo los partidos que le quedan a España (grupo A3) y las fases futuras.
- **Fórmula 1**: clasificación y carrera de cada Gran Premio hasta Abu Dabi, más el sprint de Singapur.
- **Victoria's Secret Fashion Show** (18 oct en Los Ángeles, madrugada del 19 en España).

Tiene vista de calendario mensual, vista de lista y filtros por tipo de evento. Se adapta al móvil y al modo oscuro.

## Ver el calendario

- **En local:** abre `index.html` en el navegador. No necesita servidor ni dependencias (solo carga las tipografías de Google Fonts).
- **En GitHub Pages:** en el repositorio ve a *Settings → Pages*, elige *Deploy from a branch*, rama `main` y carpeta `/ (root)`. La web quedará en `https://<tu-usuario>.github.io/<nombre-del-repo>/`.
- **En PDF:** [`calendario-otono-2026.pdf`](calendario-otono-2026.pdf) (3 páginas de mes y el detalle de cada evento).

## Contenido del repositorio

| Archivo | Para qué sirve |
| --- | --- |
| `index.html` | La web completa en un solo archivo (HTML, CSS y JS). |
| `events.json` | Los 39 eventos como datos: fecha, hora, categoría, título, detalle y lugar. |
| `calendario-otono-2026.pdf` | Versión para imprimir o compartir. |

## Cómo editar los eventos

Los eventos están dentro de `index.html`, en el bloque `<script>`, como llamadas a `add(...)`:

```js
add("2026-10-06", "20:45", "nl", "Croacia–ESP", "Croacia – España", "Jornada 4 · Grupo A3 de la Liga A.", "Estadio Poljud, Split");
//   fecha         hora     cat.  etiqueta corta  título            detalle                              lugar
```

Categorías: `lol`, `nl`, `f1`, `vs`. La fecha y la hora son las de España. Si un evento cae de madrugada (por ejemplo, Las Vegas), pon el día en que ocurre en España.

## Notas sobre los datos

- Datos recopilados el 5 de octubre de 2026. Los horarios pueden cambiar, así que confirma siempre en las fuentes oficiales: Riot / LoL Esports, RFEF y UEFA, Formula 1 y Victoria's Secret.
- Mundial de LoL: el sorteo del Play-In es el 10 de octubre. Los cruces de la fase suiza y de las eliminatorias dependen de los resultados, por eso el calendario indica los equipos que participan en cada fase y no los emparejamientos. Las horas se calcularon desde la hora oficial de Riot en el Pacífico.
- Nations League: faltan por confirmar las sedes de Chequia–España y España–Inglaterra, y las fechas de cuartos y final a cuatro de 2027.
- F1: las horas de clasificación de México y Las Vegas pueden variar una hora entre fuentes; se usó la hora oficial publicada por la F1.
- Victoria's Secret: la sede exacta y parte de la cartelera musical aún no se han anunciado.
