# Trello
Gestor de proyecto y tareas. Es un gestor multidispositivo, sencillo de utilizar.

## Tableros
Se pueden crear diferentes tablaros para cada proyecto
### Listas
Se pueden crear varias listas donde se definiran las tareas, y mover estas entre las listas
    
    ej: TODO - In Progress - DONE
### Tareas
Son las tarjetas que se crean en cada lista, y contienen unas funciones a realizar
## Equipos
Los equipos pueden tener acceso a los tableros, de forma que quedan compartidos para un grupo de personas.

# Editores
# Servidores locales
# Introducción HTML5
## ¿Qué es?
HTML (HyperText Markup Language) es un lenguaje de etiquetas que permite incluir o hacer referencia a todo tipo de información.
Los navegadores interpreten un documento de este tipo y dibuja los elementos de una página web.

    <etiqueta>contenido</etiqueta>
    
En el documento HTML debe aparecer información correctamente individualizada, de modo que al leer una página HTML comprendamos su significado. La misión de HTLM5 es mantener sólo contenido e información semántica en HTML5. Separación de la presentación del contenido.

    Ej: <b> <strong>

## Estructura de etiquetas HTML

### Etiquetas
    <etiqueta atributo="valor">contenido</etiqueta>

Existen palabras reservadas para las etiquetas, estas no se forman con cualquier palabra.
Es recomendable y buena practica escribirlas en minusculas.
Las etiquetas se abren y se cierran.
Ver tabla de etiquetas.

### Atributo 
Algunas etiquetas tienen atributos específicos que pueden ser opcionales u obligatorios. El atributo va despues del nombre de la etiqueta y determina información de esta. Una etiqueta puede tener varios atriburos, pero no se debe repetir el atributo en la misma etiqueta.
Hay 3 tipos de atributos:
#### Conjunto finito de valores
Valores ya fijados. Cualquier otro valor seria no valido.
#### Valores libres
Acepta cualquier valor, URL o texto.
#### Valores booleanos
Solo permite verdadero o falso.

### Contenido de la etiqueta
Es la información que quereos que sea afectada por dicha etiqueta.
Una etiqueta puede contener desde un fragmento de texto hasta un conjunto de etiquetas.

## Atributos comunes
Hay varios pero yo me quiero centrar en id y class. Estos atributos pueden llevar cualquier nombre como valor.
El id, establece un identificador a la etiqueta y debe ser unico en todo el documento.
El class, establece un género o tipo a una etiqueta, y puede repetirse las veces que sea necesario por todo el documento.

Estos atributos se suelen utilizar para dar aspectos en CSS, para actualizar su valor desde JS, accesos rapidos.

## Estructura del documento HTML
Un documento HTML debe tenet siempre una estructura inicial, con algunas etiquetas y características obligatorias y otras recomendadas.
### Tipo de documento
En la primera linea del documento debe ir especificado siempre de que tipo de documento HTML se trata.
HTML5: <!DOCTYPE html>
HTML4 o XHTML: <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">

En caso de no indicar el tipo de documento, el navegador entra en Quirk mode, modo de retrocompatibilidad con pag. antiguas, que procesará de forma diferente muchas etiquetas HTML o propiedades CSS.

### Head 
Hay una primera sección donde se especificarán todos los metadatos del documento. No es visual en el navegador.
En este apartado se indicanmetadatos como el título y descripción de la página o elementos relacionados que no se representaran visualmente en el navegador. También es donde se relaciona el documento con otros documentos externos, como CSS o scripts.

### Body
La segunda sección es el cuerpo de la página, donde si aparecen todos los elementos que aparecerán visualmente en el navegador del usuario.

Tanto el head como el body tienen que ir dentro de la etiqueta <html>

## Validación HTML
Existen validadores para saber los errores que tiene una web.
En nuestro caso instalaremos un plugin en atom.

## Etiquetas de texto
### fragmento de texto
### modificación de significado

## Etiquetas de agrupación
Etiquetas que se utilizan para agrupar y organizar información.
* pre: para mostrar texto respetando el formato con el que ésta escrito. También se usa junto con la etiqueta <code> anidada.
    En el caso de crear bloques de código, suele ser buena práctica incluir un atriburo class con el lenguaje usado. No es una funcionalidad de HTML5, pero muchas librerias JS nos permiten resaltar la sintaxis.
* blockquote: con el atributo cite para indicar la referencia externa. un parrafo con la cita. una sección semántica (pie cita) que contiene referencias al autor de la cita y titulo de la pelicula.

### Etiquetas para listas
* <ul> sin orden <ol> con orden y esta ultima permite varios atributos opcionales para modificar la forma de ordenarlos. para cada item se usa la etiqueta <li>

## Enlaces o hipervinculos
Una de las etiquetas mas importante de HTM es <a>. 
Se utiliza para crear enlaces, vinculos o hipervinculos. La idea es establecer una referencia a una direccion o URL que queremos mostrar.
Debe tener como minimo el atributo href, donde se especifica la direccion al documento.

### Partes de una URL
#### Protocolo: 
Existen varios tipos y es la parte inicial de la URL, el mas utilizado es http:// y el https:// para cifrar información. Al escribir la URL no debemos olvidarnos del protocolo ya que el vinculo podria no funcionar correctamente.

#### Dominio:
El dominio se compone de un subdominio (opcional), el nombre del dominio y el dominio de nivel superior o TLD.
www -> subdominio utilizado tradicionalmente para las webs.
.com .net .org . es .com.es .cat y otras -> TLD para los sitios webs.

#### Ruta: 
Es equivalente a las carpetas o directorios donde almacenamos nuestros archivos.

#### Pagina web:
El documento html, fichero con la extencion .html

#### Ancla:
Fragmento de tecto pecedido del caracter #
El navegador busca la etiqueta HTML que tenga un atributo id con ese tecto y posiciona al usuario en esa parte de la pagina.
opcional

### Rutas alternativas o absolutas
ver transparencia

## Etiquetas semanticas
En versiones anteriores se solia utilizar <div> para hacer las agrupaciones de secciones y para identificarrlas y quedara un poco mas claro se añadian los atributos id y class.
En HTML5 se introducen una serie de etiquetas de agrupacion que funcionan igual que el <div> pero que ademas tienen un significado semantico ya que indican la naturaleza del contenido que agrupan.
Esto ayuda a que cualquier navegador, robor de biscador o aplicaicon o sistema informatico sea capaz de leer el documento y conocer perfectamente la naturaleza de dicha seccion.

-> 100% recomendable escuchar http://wecodesignpodcast.com/2017/09/05/accesibilidad-practica/

## Etiquetas de tablas
Etiquetas basicas para crear tablas de la forma mas sencilla posible.
<table> <tr> <td> <th>
    
### Combinar celdas de una tabla
Cada etiqueta <td> y <th> puede incluir una serie de atributos para modificar su comportamiento o para establecer relaciones semanticas entre celdas. Probablemente, las mas interesantes sean colspan y rowspan.
Esto sirve para poder indicar que ciertas columnas/filas abarque mas espacio y se combinen.
    
Tambien existen unas etiquetas para la organizacion de tablas 
<thead> para la cabecera, con cada columna
<tbody> para el cuerpo de la tabla, cada celda.
<tfoot> pie de la tabla
    
## Etiquetas de imagenes
Hay que tener en cuenta que pueden haber dos tipos: de contenido o de decoracion
De contenido se indican con la etiqueta <img> para las de decoracion lo mejor es utilizar CSS para esto.
Los atributos src y alt son obligatorios. Los tamaños no son necesarios.
Formatos soportados PNG JPG SVG GIF...

## Etiquetas de audio
Se usa la etiqueta <audio> y el atributo src obligatorio. Existen otros atrobutos para que precarge, se auto-reproduzca, pare, etc
    
## Etiquetas de video
Se usa la etiqueta <video> y se utiliza igual que la de audio.
Tener en cuenta que para videos externos como pueden ser Youtube/Vimeo etc, es necesario usar la etiqueta <iframe> en lugar de la de video
    
No hacer autoplay, preferiblemente, sobretodo los sonidos
    
## Etiquetas de cabecera
<head> contiene etiquetas de metadatos documentos.

### Titulo y codificacion
Es recomendame meter en el <head>  minimo las siguientes etiquetas:
    <title> titulo de documento</title>
    <meta charset="utf-8">
   
Importante utilizar siempre la misma codificacion en todos los documentos. Evitando problemas con vocales acentuadas o caracteres con ñ, ¿, ¡ u otros.
Para evitar problemas de codificacion, incluir el meta indicado, guardar el archivo HTML con codificacion UTF-8

### Favicons 
No esta definida en las especificaciones por lo que cada navegador (y sistema operativo) la implementa como quiere. Hay navegadores que solo soportan favicon en formato PNG otros que solo soportan unas resoluciones... 
Recomendable https://realfavicongenerator.net/

## Etiquetas de metadatos
Atraves de los atributos name y content podemos indicar una gran cantidad de metadatos al documentos.

## Etiquetas interactivas
En dichas etiquetas el usaurio debe tomar parte de forma activa para activarlas o utilizarlas. Son elementos desplegables, menus contextuales, dialogos emergentes, etc..
    
