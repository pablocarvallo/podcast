# Por escuchar

App personal para iPhone que muestra solo los episodios sin escuchar de los podcasts elegidos entre los que sigues en Apple Podcasts. Una lista por fecha, un reproductor sencillo y nada más.

## Qué hace

- **Elige tus programas**: la primera vez lee la lista de programas que sigues en Podcasts y te deja marcar los que quieres ver.
- **Lista de pendientes**: episodios ordenados del más nuevo al más antiguo, agrupados por día (Hoy, Ayer, el día de la semana o la fecha). Arriba, las portadas de tus programas con el número de pendientes; al tocar una se filtra la lista.
- **Marcar como escuchado**: desliza un episodio hacia la izquierda, o márcalo desde el reproductor. Siempre se puede deshacer.
- **Reproductor**: toca un episodio para escucharlo en la app, con avance guardado, retroceso de 15 s, avance de 30 s, velocidad (1× a 2×) y controles en la pantalla bloqueada. Al terminar un episodio, queda marcado como escuchado. **Abrir en Podcasts** lo abre en la app nativa.
- **Agregar programas**: en **Programas → Agregar programas** aparecen los programas que sigues en Podcasts y que aún no están en la app. Si seguiste programas nuevos después, **Actualizar desde Podcasts** vuelve a leer la lista. También se puede buscar un programa por nombre.
- **Ajustes**: cuántos días hacia atrás mostrar (7, 14, 30 o 90), marcar todo como escuchado, y quitar un programa o ponerlo al día con el botón **⋯**.

## Cómo sabe qué está sin escuchar

Apple no permite que otras apps lean la biblioteca de Podcasts ni qué episodios ya escuchaste. Por eso:

1. La lista de programas que sigues llega con un atajo de la app Atajos (abajo).
2. Los episodios se consultan en el directorio público de Apple Podcasts, el mismo que usa la app nativa. No se necesita cuenta ni clave.
3. Un episodio está pendiente si se publicó dentro de los días elegidos en Ajustes y no lo has marcado como escuchado en esta app.

La primera vez, la lista trae todos los episodios recientes. Si ya los escuchaste en Podcasts, toca **Partir desde hoy** y solo verás los que se publiquen desde ese momento. Lo mismo se ofrece al agregar programas nuevos.

Lo que escuches en la app Podcasts no se descuenta aquí solo: márcalo deslizando el episodio.

## El atajo «Mis podcasts»

Se crea una vez en la app **Atajos**:

1. Abre **Atajos**, entra a **Atajos** y toca **+**.
2. Toca el nombre arriba, elige **Renombrar** y escribe **Mis podcasts**, tal cual.
3. En el buscador de acciones escribe **podcast** y agrega **Obtener podcasts de la biblioteca**.
4. Agrega **Obtener detalles del podcast**. Toca el detalle en azul y elige **ID de la tienda** (Store ID).
5. Busca y agrega **Combinar texto**. Toca el separador en azul y elige **Nueva línea**. Sin este paso, el portapapeles entrega solo el primer programa.
6. Busca y agrega **Copiar al portapapeles**, después de **Combinar texto**.
7. Toca **OK**. La primera vez que se ejecute, iOS pedirá permiso para usar Podcasts: toca **Permitir**.

Los nombres de las acciones pueden variar un poco según la versión de iOS; buscar «podcast» las muestra todas.

**Uso:** en la app toca **Abrir el atajo** (o **Actualizar desde Podcasts**). Cuando el atajo termine, vuelve a la app con **◀** arriba a la izquierda y toca **Pegar lista**. iOS mostrará el botón **Pegar** para autorizar la lectura del portapapeles.

La app entiende lo que copie el atajo en cualquiera de estas formas: un ID por línea (lo recomendado), enlaces de Apple Podcasts o nombres de programas. Los encontrados por nombre se marcan como «Encontrado por nombre» para revisarlos.

Los programas que no están en el directorio de Apple (por ejemplo, suscripciones privadas agregadas con un enlace RSS) no se pueden mostrar.

## Instalar en el iPhone

1. Abre **https://pablocarvallo.github.io/podcast/** en Safari.
2. Toca **Compartir** y luego **Agregar a inicio**.

Se abre a pantalla completa con su icono, como las otras apps.

## Datos

Todo queda guardado solo en el iPhone (almacenamiento local de la app): los programas elegidos, los episodios marcados como escuchados, el avance de cada episodio y los ajustes. Nada se envía a otro servidor. Las consultas a Apple Podcasts solo piden los episodios públicos de cada programa.

Los episodios se actualizan al abrir la app (como máximo cada 15 minutos por programa) o con el botón de actualizar. Apple puede tardar algunas horas en incluir un episodio recién publicado en su directorio.

## Archivos

| Archivo | Contenido |
| --- | --- |
| `index.html` | La app completa: pantallas, estilos y lógica |
| `manifest.webmanifest` | Nombre, colores e iconos para instalarla |
| `sw.js` | Guarda la app y las portadas para abrirla sin conexión |
| `icons/` | Icono en SVG y PNG (1024, 512, 192 y 180 px) |

## Icono

Un punto blanco con dos ondas sobre azul cobalto: el episodio pendiente que «suena». Archivo fuente en `icons/icon-full.svg`.
