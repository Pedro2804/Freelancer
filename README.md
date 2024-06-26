# Freelancer

/*----------Haces que cada rem valga 10px----------
html{ font-size: 62.5%; }

body{ font-size: 16px; }
__________________________________________________
----------Elimina el problema de afectar el tamaño de un contenedor al palicar padding o margen----------
html{ box-sizing: inherit;}

*, *:before, *:after{ box-sizing: inherit; }
__________________________________________________
----------Selectores----------
- * Universal, selecciona todos los elementos del HTML. Ejemplo:
    *{}
- Elemento -> Selecciona un elemento en base a su etiqueta. Ejemplo:
    h1{}, p{}, div{} etc.

- Clase -> Es reutilizable y se inicia con un punto. (Como si renombraramos una equiqueta) Ejemplo:
    .cliente{}, .user{}, .caja{} etc.
    Tambien se puede seleccionar más de 2 elementos usando una ',', para evitar codigo duplicado. Ejemplo:
    .titulo, .subtitulo{}

- ID -> No es reutilizable, es único en cada documento e inicia con #. (Como si renombraramos una equiqueta) Ejemplo:
    #cliente{}, #user{}, #caja{} etc. El nombre tiene que ir más a corde a lo que representa la etiqueta.

- Atributo -> Selecciona elementos basados en algún atributo que tengan. Ejemplo:
    [src="logo.png"]{} etc.

- Combinación de descendentes -> Selecciona los elementos hijos cuyo padre sea una clase (o ID) en específico. Ejemplo:
    .cliente .nombre{}, .clase #id{}, .clase h1{}, div [src="logo.png"]{} etc.

- Todos los hijos -> Aplica la siguiente regla a todos los parrafos hijos. Ejemplo:
    .cliente > p{}, #cliente > p{}, div > p{} etc.

- Seudo selectores -> son elementos que no existen en html. Es una forma de almacenar variables (coustom propetys).
    :root{
        --fondo: #ffffff
    }
Para usarlo se usa var(--fondo)

- Seudo selectores after y before ->  son elementos que puedes usar para colocar contenido antes o despues de un contenidos.
_____________________________________________________
----------Especificidad----------
Mientras más especifico sea el selector, será el estilo que se va a tomar.
CSS es en cascada pero no significa que el ultimo selector será tomado en cuenta, si no que va a tomar el selector más específico.
    h1.titulo span{} es más especifico que
    .titulo span{}

NOTA: 'important!' pasa por encima de todo. Sin imporrtar que tan específico sea un selector, va a tomaren cuenta la que tenga !important.
    .clase{color: red!important;} es más específico que
    h1#id span{color: blue;}
______________________________________________________
----------Display----------
- Block -> Significa que el elemento se colocará uno debajo del otro sin importar tamaño o contenido.
- Inline -> Significa que el elemento se posicionará a la derecha una vez que haya tomado el espacio que requiera.
- Flex-box -> se tiene que poner en el elemento padre.
    ~ Se tiene acceso a una dimencióm, row o column
- Grid -> Permite definir la ubicación y tamaño de los elementos de tu sitio web.
    ~ El contenido se agrupa dentro de un área definida.
    ~ Es como una tabla de HTML, con la ventaja de mayor flexibilidad y control sobre tu diseño. 
    ~ Con acceso a las 2 dimenciones al mismo tiempo
    grid-template-columns: 26rem 26rem 26rem; Defines el tamaño de cada columna que se ocupe
    grid-template-rows: 20rem 20rem; Defines el tamaño de cada fila que se ocupe

    grid: 20rem 20rem / 26rem 26rem 26rem; Lo mismo que los anteriores, a la izquierda van las filas y a la derecha columnas

¿Cuándo usar grid o flex-box?
- flex-box -> Para alineación o distribución de los elementos que estarán dentro de los contenedores.
    ~ Por ejemplo: En tun nav.
- grid -> Para definir el layaut de tu sitio web, como pueden ser las columnas o contenedores de elementos.
    ~ Por jemplo: Para distribuir todos los elementos del html.

- margin: 0 auto -> tambien sirve para centrar y es conveniente usarlo cuando el padre del elemento a centrar no es un display: flex;
    De tipo block

NOTA: No es necesario especificar un display, salvo que se quiera modificar el que viene por default.

----------CSS box model----------
El tamaño de lo que se muestra en pantalla está delimitada por 4 cosas:
- Tamaño del contenido.
- Tamaño de relleno (padding).
- Tamaño del borde.
- Margen
___________________________________________________
*/
