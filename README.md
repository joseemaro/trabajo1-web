# Trabajo Practico 1
## Parte Teorica

**1. ¿Qué es un lenguaje de marcado? ¿Cuál es su utilidad? ¿Qué es un tag? ¿Qué es un atributo?**

Markup Language hace referencia a un lenguaje que se basa en etiquetas que uno agrega a un texto para darle estructura e información adicional. A diferencia de los "Lenguajes de Scripting" que se usan para crear programas informáticos, los lenguajes de marcado son sólo reglas para ordenar un documento. Por lo tanto, podemos decir que, HTML no es un lenguaje de programación; es un lenguaje de marcado que define la estructura de tu contenido.
Un tag es el elemento que utilizamos para encerrar diferentes partes del contenido para que se vean o comporten de una determinada manera. Es decir, un elemento HTML se separa de otro por medio de "etiquetas", las cuales consisten en elementos rodeados por "<" y ">".
Los elementos pueden también tener atributos. Estos contienen información adicional acerca del elemento, la cual no queremos que aparezca en el contenido real que se va a mostrar. 
Un atributo debe tener siempre:
	Un espacio entre éste y el nombre del elemento (o del atributo previo, si ya posee uno o más atributos).
	El nombre del atributo, seguido por un signo de igual (=).
	Comillas de apertura y de cierre, encerrando el valor del atributo.


**2. ¿Qué es un lenguaje de marcado? ¿Cuál es su utilidad? ¿Qué es un tag? ¿Qué es un atributo?**

HTML, que significa Lenguaje de Marcado de Hipertextos (HyperText Markup Language), es la pieza más básica para la construcción de la web y se usa para definir el sentido y estructura del contenido en una página web. El conjunto mínimo de tags que debe tener toda página son los siguientes:

<!DOCTYPE html>
<html>
<head>
    <title>Título de la página</title>
</head>
<body>
 …   
</body>
</html>

	La declaración DOCTYPE le avisa al browser que el documento que va a leer es HTML.
	El texto entre <html> y </html> define donde empieza y donde termina el documento HTML.
	El texto entre <head> y </head> provee información sobre el documento llamada meta data, data sobre la página pero que no forma parte de su contenido visible.
	El texto entre <title> y </title> provee un título para el documento: lo que aparece escrito en la tab del navegador, y el texto que muestra Google en sus resultados de búsqueda. Google (o el motor de búsqueda que prefiramos) utiliza esta meta data para entender de qué se trata nuestra página y decidir como rankearla (no es el único factor, toma muchísimos más).
	El texto entre <body> y </body> describe el contenido visible del documento, lo que el navegador le mostrará al usuario. Por ejemplo, podríamos cologar tags <h1> los cuales describen un encabezado, o tags <p> que describen un párrafo.


**3. ¿Cuál es la utilidad e importancia de los enlaces o links entre páginas? ¿Qué significa hipertexto? ¿Un link solo puede apuntar a otra página? ¿Qué importancia tiene esto último?**

Los links son un aspecto fundamental de la web. Al subir contenido a Internet y vincularlo a páginas creadas por otras personas, te haces participante activo en la red mundial (World Wide Web). Por otro lado, "Hipertexto" se refiere a los enlaces que conectan las páginas web entre sí, ya sea dentro de un mismo sitio o entre diferentes.
El atributo href que se utilizan dentro de los tag <a> o <link> por ejemplo, se usa para indicar la dirección a donde deberá llevar el link cuando el usuario haga click. Este atributo puede linkear tanto a páginas locales como a páginas externas en internet. Pero, aparte de esto, un link no necesariamente apunta siempre a una página diferente, sino que pueden usarse para direccionar a secciones dentro de una misma página, o bien estar vacío. Básicamente, esto es importante porque hay ocasiones en las que no queremos si o si dirigir a determinado “lugar” sino que debemos utilizar los vínculos para ejecutar alguna instrucción y no para dirigirnos a una página.

**4. ¿Cómo funcionan los tags audio y video?**

Antes de HTML5, los archivos de audio y video solo se podían reproducir en un navegador con un complemento (como flash).
El tag <audio> especifica una forma estándar de incrustar audio en una página web. El mismo puede contener:
	El atributo controls permitirá que el usuario controle la reproducción de audio, incluyendo volumen, búsqueda y pausar/reanudar reproducción.
	El tag <src> (dentro del opening y closing tag) contiene la URL del audio que se va a insertar.
	Autoplay es un atributo booleano que hará que el sonido comience a reproducirse automáticamente en cuanto sea posible.
	Buffered es un atributo que se puede leer para determinar qué intervalos de tiempo del multimedia se han almacenado en búfer. Este atributo contiene un objeto TimeRanges.
	Preload error 548523. El objetivo de este atributo enumerado es proporcionar una sugerencia al navegador sobre qué cree el autor que proporcionará la mejor experiencia para el usuario.
Luego, tenemos el tag <video> que básicamente funciona con los mismos atributos y tags que <audio> pero se agrega: 
	Height: la altura del área de visualización del vídeo en píxeles CSS.
	Loop: un atributo booleano; si se especifica, al alcanzar el final del video, volverá automáticamente al principio.
	Width: la anchura del área de visualización del vídeo en píxeles CSS.

**5. ¿Qué es el Rendering Engine de un Browser? ¿Cuál es el que utiliza cada uno de los 5 browsers más conocidos (Chrome, Firefox, Safari, IE-Edge, Opera)? ¿Cuál es la importancia de conocer cada uno de ellos en la construcción de un sitio?**

El motor de renderizado web es un software que se encarga de tomar información del formato (contenido en el código no visible de una página web), lo interpreta (renderizado) y realiza una representación visual del mismo (lo muestra).
El motor de renderizado va a interpretar las marcas (en HTML, XML, archivos de imágenes, etc.) o la información de formato (como CSS, XSL, etc.), para mostrar el contenido formateado (es decir, con las formas y estilos apropiados).
Motores de los principales navegadores:
	Gecko, utilizado en Mozilla Suite.
	Blink, utilizado en Google Chrome, Microsoft Edge (desde 2020) y opera.
	WebKit, el motor de Epiphany, Safari.
	Tasman, el motor de Internet Explorer para Mac.
Importancia de sus diferencias:
La manera en que se maneja la seguridad de las aplicaciones web es algo que cada motor de navegador maneja de forma relativamente diferente.
La forma en que el código dinámico se procesa y optimiza es diferente entre los motores, y tiene un impacto en la rapidez con que aparece una página.
Todos tienen diferencias en cómo se actualizan las aplicaciones web, como maneja la memoria y el tiempo del núcleo de la CPU y cómo responde a los fallos del sistema.
Hay diferencias importantes para los desarrolladores: la rapidez con que se puede agregar y aprobar el código, los procedimientos para corregir errores, la cercanía del motor del navegador con el navegador real (los usuarios finales no notarán esto).