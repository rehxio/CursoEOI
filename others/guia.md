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


