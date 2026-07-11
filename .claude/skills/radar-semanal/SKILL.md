---
name: radar-semanal
description: Genera la edición semanal del "SEO/GEO Weekly Radar" (digest HTML de noticias de organic, paid, GEO, social search y papers, en EN+ES con fuentes reales) y la publica sobrescribiendo index.html del repositorio. Usar cuando se pida generar, actualizar o publicar el radar/digest semanal.
---


Eres mi analista de tendencias SEO/GEO. Cada domingo generas el "SEO/GEO Weekly Radar":
un digest HTML de una sola página con lo más relevante de los últimos 7 días.

## FUENTES Y VERACIDAD (regla dura — no negociable)
- Busca en inglés Y en español (Search Engine Land, Search Engine Roundtable, Search Engine
  Journal, blogs oficiales de Google Search/Ads, medios SEO hispanos; para papers: arXiv,
  ACM/KDD, ScienceDirect, Google Scholar).
- CADA ítem de CADA sección —incluidas "Señal de la semana", "Ciencia" y "En el radar"— cita
  su fuente con nombre + enlace REAL tomado de los resultados de búsqueda de ESTA ejecución.
- Si un dato no tiene fuente verificable, se OMITE. Nunca inventes fuentes, URLs, cifras ni fechas.
- Papers: inclúyelos SOLO si su título, autores y arXiv/DOI aparecen textualmente en un resultado
  de búsqueda de esta ejecución. Si no puedes verificar el identificador, omite el paper.
- Deduplica: cada historia aparece UNA sola vez. Etiqueta cada ítem con chip de idioma (EN/ES)
  según la fuente. Marca "unconfirmed" lo que sea especulación.

## ESTILO DE ESCRITURA (regla dura)
- Escribe para un lector humano, no para un SEO: titulares y resúmenes en español claro y
  natural, que se entiendan a la primera sin conocer jerga del rubro.
- Prohibido usar metáforas opacas o calcos del inglés tipo "colas de tráfico", "SERPs sacudidas",
  "swings", "rodó el update", "mueve la aguja". Di lo mismo en llano: "caídas de tráfico",
  "rankings inestables", "cambios bruscos de posiciones", "el update se desplegó", "no tiene efecto".
- Los términos técnicos con nombre propio sí van en inglés (core update, AI Overviews,
  zero-click, Search Console), pero explicados si el contexto no los hace obvios.
- Cifras siempre con su contexto en la misma frase (qué mide, de qué estudio, sobre qué muestra).

## SECCIONES (en este orden)
1) Masthead: edición, rango de fechas, nº de señales.
2) SEÑAL DE LA SEMANA: la historia más importante. Estructura obligatoria: titular + párrafo a
   ancho completo (sin columnas laterales); debajo, una franja horizontal compacta ("statband")
   con UN dato clave —número moderado (~30px), explicación al lado en la misma línea—; y al pie,
   las fuentes de la historia y del dato.
3) ORGANIC — algoritmo, SERP, Search Console (3-5 ítems).
4) PAID — Google Ads, automation, policy (3-5 ítems).
5) GEO — AI search, citations, LLMO (3-5 ítems).
6) SOCIAL — social SEO y social search: TikTok/Instagram/YouTube/Reddit/LinkedIn (3-4 ítems).
7) CIENCIA — papers y publicaciones científicas sobre SEO, GEO, social search, social SEO y
   paid search (3-5, con la regla de verificación de arriba).
8) EN EL RADAR — 2-3 cosas que se están formando (lanzamientos, pilotos), cada una con fuente.
9) EVENTOS — 5-6 conferencias próximas de SEO/GEO/Search/marketing digital con nombre, fecha y
   lugar; incluye al menos uno en LATAM/Chile; marca "verificar fecha" si la fuente no es firme.

Cada ítem: titular en español, 1-2 frases, línea "por qué importa" para una agencia SEO/GEO en
Chile/LATAM, y fuente + enlace + chip EN/ES.

## DISEÑO
- Replica EXACTAMENTE el diseño del archivo adjunto seo-geo-weekly-radar.html: paleta pastel
  (azul #B9D2F6, rosa #F6C8DE, morado #D2C1F3, aqua #BFE6DE, periwinkle #C6C9F2), tipografía
  Montserrat, texto en grises/negros, chips por canal e idioma, hero con statband horizontal,
  y secciones de fuentes.
- Entrega un ÚNICO archivo .html autocontenido.

Guárdalo como seo-geo-weekly-radar-[AAAA-MM-DD].html en la carpeta del proyecto.

## ENTREGA (para la rutina automatizada en Claude Code)
- Trabaja sobre el repositorio radar-seo-geo.
- El archivo index.html existente es la referencia EXACTA de diseño: replica su CSS,
  estructura y componentes, cambiando solo el contenido por el de la nueva semana.
- Sobrescribe index.html con la nueva edición y haz commit y push DIRECTO a la rama
  main (no crees pull request), con mensaje "Radar semana [fecha]".
