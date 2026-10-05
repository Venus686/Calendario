# 🍂 Calendario de otoño 2026

> Todo lo que hay que ver de octubre a diciembre en un solo sitio, **en hora de España**.

![Hora](https://img.shields.io/badge/hora-Espa%C3%B1a%20peninsular-8e7cf5?style=flat-square)
![Eventos](https://img.shields.io/badge/eventos-39-f26b5b?style=flat-square)
![Modo oscuro](https://img.shields.io/badge/modo%20oscuro-s%C3%AD-2fa68a?style=flat-square)
![Sin dependencias](https://img.shields.io/badge/dependencias-ninguna-e5559a?style=flat-square)

📄 **[Descargar el PDF](calendario-otono-2026.pdf)** · 🌐 **[Abrir la web](index.html)**

---

## ✨ Qué incluye

| | Evento | Fechas | Qué hay |
| :-: | --- | --- | --- |
| 🟣 | **Mundial de LoL** | 15 oct – 14 nov | Play-In (15–18 oct), fase suiza (23–31 oct), cuartos y semis (3–8 nov) y gran final (14 nov, Brooklyn) |
| 🔴 | **Nations League** | 6 oct, 12 nov y 15 nov | Solo los partidos de España en el grupo A3: Croacia, Chequia e Inglaterra. Más las fases de 2027 |
| 🟢 | **Fórmula 1** | 9 oct – 6 dic | Clasificación y carrera de los 7 Grandes Premios que quedan, más el sprint de Singapur |
| 🩷 | **Victoria's Secret Fashion Show** | 19 oct, 01:30 | Es el domingo 18 a las 16:30 en Los Ángeles, así que en España cae de madrugada |

Vista de calendario mensual, vista de lista y filtros por tipo de evento. Se adapta al móvil.

---

## 🚀 Cómo verlo

**En local:** abre `index.html` en el navegador. No necesita servidor ni instalar nada. Solo carga las tipografías de Google Fonts.

**En GitHub Pages:**

1. Sube la carpeta a un repositorio.
2. Ve a **Settings → Pages**.
3. Elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
4. La web quedará en `https://<tu-usuario>.github.io/<nombre-del-repo>/`.

---

## 🗂️ Contenido del repositorio

| Archivo | Para qué sirve |
| --- | --- |
| `index.html` | La web completa en un solo archivo (HTML, CSS y JS) |
| `events.json` | Los 39 eventos como datos: fecha, hora, categoría, título, detalle y lugar |
| `calendario-otono-2026.pdf` | Versión para imprimir o compartir |

---

## ✏️ Cómo editar los eventos

Los eventos están en `index.html`, dentro del bloque `<script>`, como llamadas a `add(...)`:

```js
add("2026-10-06", "20:45", "nl", "Croacia–ESP", "Croacia – España", "Jornada 4 · Grupo A3 de la Liga A.", "Estadio Poljud, Split");
```

Los campos van en este orden: **fecha, hora, categoría, etiqueta corta, título, detalle y lugar**.

| Código | Categoría |
| :-: | --- |
| `lol` | 🟣 Mundial de LoL |
| `nl` | 🔴 Nations League |
| `f1` | 🟢 Fórmula 1 |
| `vs` | 🩷 Victoria's Secret |

La fecha y la hora son las de España. Si un evento cae de madrugada (por ejemplo, Las Vegas), pon el día en que ocurre en España.

---

## 📌 Notas sobre los datos

- 🗓️ Datos recopilados el **5 de octubre de 2026**. Los horarios pueden cambiar, así que confirma siempre en las fuentes oficiales: Riot / LoL Esports, RFEF y UEFA, Formula 1 y Victoria's Secret.
- 🟣 **LoL:** el sorteo del Play-In es el 10 de octubre. Los cruces de la fase suiza y de las eliminatorias dependen de los resultados, por eso el calendario indica los equipos que participan en cada fase y no los emparejamientos. Las horas se calcularon desde la hora oficial de Riot en el Pacífico.
- 🔴 **Nations League:** faltan por confirmar las sedes de Chequia–España y España–Inglaterra, y las fechas de cuartos y final a cuatro de 2027.
- 🟢 **F1:** las horas de clasificación de México y Las Vegas pueden variar una hora entre fuentes. Se usó la hora oficial publicada por la F1.
- 🩷 **Victoria's Secret:** la sede exacta y parte de la cartelera musical aún no se han anunciado.
