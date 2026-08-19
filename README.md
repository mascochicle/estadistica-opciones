# Estadística de Opciones

Tablero de análisis para un registro de operaciones con opciones sobre acciones
e índices. Página estática: sin dependencias externas, sin conexiones, sin
seguimiento. Los datos van dentro del propio archivo.

**[Ver el tablero →](https://mascochicle.github.io/estadistica-trading/)**

## Qué muestra

561 operaciones cerradas, repartidas en cuatro formas de operar distintas:

- **Seminario 1** — primera parte del curso, abril 2025
- **Seminario 2** — segunda parte, agosto 2025; entre una y otra hay dos meses sin operar
- **0DTE** — opciones que vencen el mismo día, sobre SPX y SPY
- **Método propio** — criterio propio, mezcla de lo anterior con análisis técnico

Cortes disponibles: por grupo, por plazo comprado, por estrategia, por
subyacente, por mes y por tipo de cierre (vendida o expirada sin valor).

## App de captura

Además del tablero, el repositorio sirve una pequeña app instalable para anotar
la estrategia **en el momento de abrir** una operación — que es lo único que el
extracto del bróker no puede saber.

**[Abrir la app →](https://mascochicle.github.io/estadistica-trading/captura/)**

Es una PWA: se instala en el teléfono, funciona sin señal y guarda en el propio
aparato. Dos toques por operación; el resto de los datos llegan del extracto.

## Cómo está hecho

Un solo archivo HTML. Las gráficas son SVG generado en el navegador, sin
librerías. Funciona igual abierto desde disco que servido por HTTP.

El origen de los datos es un extracto de actividad del bróker, procesado a una
bitácora en Excel donde se anota la estrategia de cada operación; de ahí sale el
conjunto de datos que va embebido en la página.

## Aviso

Esto es un ejercicio de análisis de datos. No es asesoría de inversión ni una
recomendación de ninguna estrategia. Las opciones pueden perder el 100% de su
valor.
