# Sesión 1

1. Lo que quería conseguir: cargar los datos del Combine, construir una base
   de análisis y probar si la propuesta del analista jefe (quitar todos los
   faltantes) era buena idea.
2. Archivos y código: sesion1_trabajo.Rmd (carga nfl_data.csv, construye
   la base de análisis y, al final, la parte A).
3. Comprobaciones que hice: conté las filas antes y después de filtrar
   (de 3,197 a 1,596). El archivo compila con Knit. Comparé las dos bases por
   posición, career_av, Pro Bowl y jugadores de primera ronda.
4. Cambios que conservé o descarté: descarté la propuesta del analista jefe
   porque casi elimina a los QB (95% de los QB no hacen bench press).
   Conservé una alternativa sin bench_press, que guarda 2,061 jugadores.
5. Lo que puedo afirmar: quitar todos los faltantes no da una base "limpia",
   da una base con sesgo. Los faltantes no son al azar: dependen de la posición.
   Por eso es mejor no pedir bench_press.
