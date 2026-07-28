# QuarxAI News

Este repositorio contiene los datos publicos que alimentan la seccion "News" del sitio de QuarxAI (https://quarxai.io/news.html).

El sitio consume quarxai-news-data.json directamente desde este repo (via raw.githubusercontent.com), sin necesidad de un redeploy del sitio: alcanza con actualizar el JSON aqui para que el cambio se refleje en produccion.

## Que es

Un resumen periodico y curado de novedades de la industria de IA aplicada a salud mental / bienestar emocional: regulacion, competidores, seguridad e incidentes, mercado e inversion, junto con una seccion propia ("Que estamos haciendo en MindBridge") que explica como respondemos desde el producto. Cada entrada incluye version en espanol e ingles.

## Esquema de quarxai-news-data.json

Cada entrada dentro de entries tiene esta forma (simplificada): id, date, period, title, dek, sections (lista de heading mas body: Regulacion, Competidores, Seguridad e incidentes, Mercado e inversion), sources (lista de title mas url), our_response (heading mas body: Que estamos haciendo en MindBridge), y en (la misma estructura completa traducida al ingles).

Las entradas nuevas se agregan al inicio del array entries, manteniendo las anteriores como historial.

## Actualizacion

Las entradas se investigan y redactan semanalmente citando fuentes reales, y se commitean directamente a este archivo.
