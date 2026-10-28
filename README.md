# Pronosticar el éxito en la NFL

Proyecto del curso "Programar con criterio en la era de la IA".
Pregunta: ¿qué características de un jugador, conocidas en el draft,
permiten pronosticar su éxito profesional?

Autora: Manuela Jaramillo Castro

## Datos
- Archivo: nfl_data.csv del repositorio phcs971/nfl-draft-dataset
  (licencia MIT), leído desde una URL fijada a la versión 54730ea.
- Contenido: datos de jugadores del draft de la NFL, con sus pruebas del Combine,
  su posición, su ronda de draft y su carrera profesional. La base que usamos
  tiene 3,197 jugadores y 33 variables.
- Base de análisis: jugadores que tienen las pruebas del Combine que usamos.
  No pedimos bench_press, porque muchos jugadores (sobre todo QB) no la hacen.

## Variables principales
- Éxito observado: career_av (Approximate Value de su carrera). Mide cuánto
  aportó el jugador en la NFL. También usamos Pro Bowl.
- Predictores: forty, vert_leap, broad_jump, bench_press, shuttle, posición
  y ronda del draft. Se conocen en el draft porque se miden en el Combine,
  antes de que los equipos elijan.

## Decisiones de limpieza
1. No usamos la base "sin un solo faltante", porque quita casi a todos los QB
   y a otros buenos jugadores. Eso crea sesgo.
2. Quitamos la condición de bench_press y pedimos solo las otras cuatro pruebas,
   para conservar más jugadores y todas las posiciones.

## Carpetas
- sesion-1/ a sesion-5/: trabajos de cada sesión
