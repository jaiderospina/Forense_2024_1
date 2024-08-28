### **Laboratorio de Administración de Kali Linux desde la Terminal**

#### **Objetivo del Laboratorio:**
Este laboratorio está diseñado para que los estudiantes se familiaricen con los comandos básicos y avanzados de administración de Kali Linux mediante ejercicios prácticos. Cada actividad tiene como objetivo desarrollar habilidades específicas de manejo de archivos, búsquedas, administración de unidades, y gestión de procesos en un entorno Linux.

#### **Requisitos:**
- Kali Linux instalado (puede ser en máquina virtual o física).
- Acceso a la terminal de Linux.
- Una memoria USB para las actividades de montaje y desmontaje de unidades.

---

### **Actividades Prácticas**

#### **Actividad 1: Creación y Manipulación de Archivos y Directorios**

1. **Crear Directorios y Archivos:**
   - Crea una estructura de directorios llamada `LaboratorioLinux` en tu directorio personal usando `mkdir`.
   - Dentro de `LaboratorioLinux`, crea tres subdirectorios: `Documentos`, `Imagenes`, `Scripts`.
   - Crea tres archivos vacíos en `Documentos`: `reporte.txt`, `notas.txt`, `resumen.doc` usando el comando `touch`.
   - Crea un archivo llamado `script.sh` en el directorio `Scripts` que contenga el siguiente contenido:
     ```bash
     #!/bin/bash
     echo "Hola, este es un script de ejemplo."
     ```
   - Verifica que los archivos y directorios fueron creados correctamente utilizando el comando `ls` con opciones adecuadas.

2. **Copiar y Mover Archivos:**
   - Copia el archivo `reporte.txt` de `Documentos` a `Scripts`.
   - Renombra el archivo `notas.txt` a `notas_renombrado.txt`.
   - Mueve el archivo `resumen.doc` al directorio `Imagenes`.

3. **Eliminar Archivos y Directorios:**

   - Elimina el archivo `reporte.txt` del directorio `Scripts`.
   - Elimina el directorio `Imagenes` junto con todo su contenido de manera segura.


#### **Actividad 2: Búsqueda y Filtros en el Sistema de Archivos**

1. **Realizar Búsquedas de Archivos:**

   - Utilizando el comando `find`, busca todos los archivos `.txt` en tu directorio `LaboratorioLinux` y subdirectorios.
   - Usa `grep` para buscar la palabra "ejemplo" dentro del archivo `script.sh` en `Scripts`.

2. **Buscar y Contar Archivos:**

   - Utiliza `find` para buscar todos los archivos que tengan más de 100 KB en el directorio `/var/log`.
   - Usa el comando `wc -l` en combinación con `grep` para contar cuántas veces aparece la palabra "error" en el archivo de registro `/var/log/syslog`.

#### **Actividad 3: Administración de Unidades y Montaje**

1. **Inspección de Unidades:**
   - Utiliza `df -h` para listar todas las particiones montadas y el espacio que ocupan.
   - Ejecuta `fdisk -l` para listar todas las particiones de los discos conectados al sistema.

Documente y explique la información presentada.

2. **Montaje y Desmontaje de Dispositivos USB:**
   - Conecta una memoria USB al equipo.
   - Usa `blkid` para identificar el nombre del dispositivo asignado a la memoria USB.
   - Monta la memoria USB en un directorio llamado `/mnt/usb` utilizando el comando `mount`.
   - Verifica que la memoria USB se haya montado correctamente ejecutando `df -h`.
   - Crea un archivo de texto dentro de la memoria USB llamado `test_usb.txt`.
   - Desmonta la memoria USB utilizando el comando `umount`.

#### **Actividad 4: Administración de Procesos y Servicios**

1. **Monitorización de Procesos:**
   - Utiliza el comando `ps aux` para listar todos los procesos en ejecución.
   - Filtra los resultados para mostrar únicamente los procesos que contienen la palabra "ssh" utilizando `grep`.

2. **Gestión de Servicios:**
   - Verifica el estado del servicio SSH en tu máquina utilizando `service ssh status`.
   - Si el servicio SSH no está en ejecución, utiliza `service ssh start` para iniciarlo.
   - Reinicia el servicio Apache2 utilizando `service apache2 restart` y verifica su estado.

#### **Actividad 5: Compresión y Descompresión de Archivos**

1. **Crear Archivos Comprimidos:**
   - Comprime el directorio `LaboratorioLinux` en un archivo `laboratorio.tar` utilizando `tar`.
   - Comprime el archivo `laboratorio.tar` en `laboratorio.tar.gz` utilizando `gzip`.

2. **Descomprimir Archivos:**
   - Descomprime el archivo `laboratorio.tar.gz` utilizando `gunzip`.
   - Extrae el contenido de `laboratorio.tar` en un nuevo directorio llamado `Restaurado`.

#### **Actividad 6: Gestión de Permisos y Propietarios**

1. **Modificar Permisos:**
   - Utiliza `chmod` para hacer que el archivo `script.sh` sea ejecutable.
   - Verifica los permisos antes y después del cambio utilizando `ls -l`.

2. **Modificar Propietarios:**
   - Cambia el propietario del archivo `script.sh` al usuario root utilizando `sudo chown root script.sh`.
   - Verifica los cambios de propietario utilizando `ls -l`.

### **Informe de Resultados:**

Cada estudiante debe documentar:
- Los comandos utilizados para cada actividad.
- Una captura de pantalla o salida de terminal que muestre el resultado de cada comando.
- Una breve explicación de lo que hace cada comando y los resultados obtenidos.

### **Conclusión del Laboratorio:**

Al completar este laboratorio, los estudiantes habrán adquirido experiencia práctica con los comandos fundamentales de administración de sistemas en Kali Linux, incluyendo la manipulación de archivos, la búsqueda avanzada, la gestión de procesos y servicios, y la administración de unidades de almacenamiento.

---
