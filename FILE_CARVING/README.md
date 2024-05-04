<a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

  <p align="center">A progressive <a href="http://nodejs.org" target="_blank">Node.js</a> framework for building efficient and scalable server-side applications.</p>
    <p align="center">


# scalpel

Programa en linea de comandos para la recuperación de archivos. 

Esta herramienta es parte de Seulkit que se integra con Autopsy

Su técnica de recuperación es el  File Carving (lee los encabezados, pies de página y estructura interna de los archivos, accediendo a la base de datos de bloques). Para ello identifica una secuencia de caracteres que algunos archivos utilizan en su comienzo y en su final. 

- Por ejemplo, un archivo JPEG utiliza la secuencia «\xff\xd8\xff\xe0\x00\x10» en su comienzo, y la secuencia «\xff\xd9» en su final.


# Sintaxis:

```
  scalpel [opciones] [dispositivo-de-entrada] -o [directorio-de-salida]
```

Antes de ejecutarlo se debe quitar el comentario a las extensiones que queramos recuperar en su archivo de configuración, que, por lo general está en /etc/scalpel/scalpel.conf. 

También la carpeta destino debe estar vacia.

Ejemplo:

En el siguiente ejemplo se ejecuta sobre la unidad /dev/sdc la cual esta dañada y se le solicita que guarde lo recuperado en la carpeta prueba

```
# scalpel /dev/sdc -o prueba
Scalpel version 1.60
Written by Golden G. Richard III, based on Foremost 0.69.

Opening target "/dev/sdc"

Image file pass 1/2.
Allocating work queues...
Work queues allocation complete. Building carve lists...
Carve lists built.  Workload:
jpg with header "\xff\xd8\xff\xe0\x00\x10" and footer "\xff\xd9" --> 0 files
Carving files from image.
Image file pass 2/2.
/dev/sdc: 100.0% |**************************************|   74.6 GB    00:00 ETAProcessing of image file complete. Cleaning up...
Done.
Scalpel is done, files carved = 0, elapsed = 648 seconds.
```

Formatos soportados
Scalpel soporta formatos de disco desde:
- FAT
- NTFS
- ext2
- particiones sin formato

Ejemplo de uso.
$ sudo gedit /etc/scalpel/scalpel.conf

Podemos ver que en el fichero está explicado el funcionamiento por RegEx (Expresiones Regulares).

Imaginemos que queremos recuperar un fichero .html que borramos accidentalmente, en la línea 162 tenemos ese ejemplo de fichero (será bueno que os leais estos ejemplos para entender el funcionamiento), en nuestro caso iremos hasta esa línea y quitaremos el comentario (simplemente bastará con eliminar el caracter # que está al comienzo de la misma).

Después de guardar las modificaciones volvemos a la consola.
Lo siguiente será indicarle al programa que los ficheros .html que hemos eliminado de nuestro disco se coloquen en un carpeta llamada “html_recovered”, y recuperaremos los datos que se encontraran en la partición /dev/sda5 (esto como repetimos es un ejemplo, podéis guardar los datos recuperados en la carpeta que queráis y buscarlos donde sea oportuno), para lo que escribiremos el comando:

```
$ sudo scalpel /dev/sda5 -o html_recovered
```

Después de un tiempo de funcionamiento, la duración dependerá del tamaño de la partición, tendremos los resultados.
En dicha carpeta existirán multitud de archivos recuperados, por lo que buscar nuestro archivo seguirá siendo como buscar una aguja dentro de un pajar. Para eliminar gran parte de los resultados, que no nos atañen buscaremos, solo por aquellos en los que nuestro usuario ha tenido algo que ver, para esto escribiremos en consola (sustituyendo USER por nuestro nombre de usuario):

```
$ sudo chown -R USER.USER html_recovered
```

Después de un poco de tiempo tendremos listos los resultados de esta criba, en la que ya nos será más sencillo localizar el archivo borrado.


## Reto 1 en clase.
•	Instalar scalpel en Windows.
## Reto 2.
•	Recuperar datos desde una USB previamente borrados.

Una vez comprendido, procedemos a descargar desde el repositorio en Github y una herramienta que será util.

•	Repositorio escalpel
•	Herramienta Ftk


Scalpel es una herramienta para utilizar en Linux como Windows, la única diferencia es que bajo Windows no puede analizar el disco, si no que debe analizar una imagen del disco, para esto, será util FTK.
Para la presente práctica, obtendremos la información de un pendrive de 2GB.

Creando una imagen con FTK

- Lo primero que haremos es pulsar el botón de “add evidence item” y elegiremos “Logical Drive”.

- Elegimos la unidad.
 
- Luego, haremos clic derecho a la unidad y seleccionamos “Export Disk Image”

- Configuramos donde se exportará la imagen.

Al concluir los pasos anteriores, estamos en condiciones de crear la imagen, solo debemos hacer clic en el boton “Start”.

Obteniendo información con Scalpel
Estamos en condiciones de buscar la información, lo primero que haremos será comprobar la ayuda, haciendo:
Visualizando la ayuda, notaremos que la sintaxis es: scalpel -opcion1 -opcion2 imagen

Algunas de las opciones mas relevantes:

- -c : Sirve para elegir el archivo de configuración. (de serie es scalpel.conf)
- -o : Sirve para elegir la carpeta donde se mandará la información. (de serie es scalpel-output)
- -v : Sirve para entrar en el verbose mode.

El archivo de configuración predeterminado trae muchas opciones para buscar gran cantidad de ficheros diferentes, solo tendríamos que ir a dicha sección y borrar ‘#’ para que dejase de ser un comentario.

Para añadir una nueva regla debemos seguir la siguiente forma: ‘extension’ y ‘tamaño’ ‘header’ ‘EOF’
Podemos buscar el header y el EOF de cada tipo de archivo por internet, para esta práctica se hará un archivo de configuración que saque todas las imagenes.

Y lanzamos el programa hacia la imagen:

Una vez ejecutado comenzará a buscar las imagenes y enviará a la carpeta que hemos indicado.

En la carpeta que hemos pasado como parámetro habrá varias carpetas con los diferentes archivos que ha recuperado y por fin hemos encontrado aquello que estabamos buscando.


Referencias:

- https://github.com/sleuthkit/scalpel
- https://youtu.be/4OkushGbBaU?si=XNCmwyaDMqcSdf6L
- https://youtu.be/0BcH2CRIVv4?si=dsKw5rEJ5KeEJtiS
- https://merchandlinux.wordpress.com/2009/03/31/recuperar-ficheros-en-linux/
- https://www.howtoforge.com/recover-deleted-files-with-scalpel




