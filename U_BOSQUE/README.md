## **Manual de Comandos para Administración de Kali Linux desde la Terminal**

### **1. Navegación y Manipulación de Archivos y Directorios**

- **`ls`**  
  Lista los archivos y directorios en el directorio actual.  
  - **`ls -l`**: Muestra una lista detallada con permisos, propietario, tamaño y fecha de modificación.  
  - **`ls -a`**: Incluye archivos ocultos (que comienzan con `.`).

- **`cd <directorio>`**  
  Cambia al directorio especificado.  

  - **`cd ..`**: Retrocede un nivel en la jerarquía de directorios.  
  - **`cd ~`**: Cambia al directorio del usuario actual.

- **`mkdir <nombre_directorio>`**  
  Crea un nuevo directorio con el nombre especificado.  
  - **`mkdir -p /ruta/completa/del/directorio`**: Crea un directorio junto con los directorios padre necesarios.

- **`touch <nombre_archivo>`**  
  Crea un nuevo archivo vacío con el nombre especificado o actualiza la fecha de modificación si el archivo ya existe.

- **`cp <origen> <destino>`**  
  Copia un archivo o directorio de origen al destino.  
  - **`cp -r <directorio_origen> <directorio_destino>`**: Copia recursivamente todo el contenido de un directorio.

- **`mv <origen> <destino>`**  
  Mueve o renombra archivos o directorios.  
  - **`mv archivo.txt /ruta/nueva/`**: Mueve `archivo.txt` al nuevo directorio.  
  - **`mv archivo.txt nuevo_nombre.txt`**: Renombra `archivo.txt` a `nuevo_nombre.txt`.

- **`rm <archivo>`**  
  Elimina el archivo especificado.  
  - **`rm -r <directorio>`**: Elimina de forma recursiva un directorio y su contenido.  
  - **`rm -i <archivo>`**: Pide confirmación antes de eliminar.

### **2. Inspección y Montaje de Unidades**

- **`df -h`**  
  Muestra el uso del espacio en disco de todas las particiones de forma legible para humanos.

- **`du -sh <directorio>`**  
  Muestra el tamaño total de un directorio de forma resumida.

- **`mount <dispositivo> <punto_de_montaje>`**  
  Monta un dispositivo o una partición en el sistema de archivos.  
  - **`mount /dev/sdb1 /mnt/usb`**: Monta la partición `/dev/sdb1` en `/mnt/usb`.

- **`umount <punto_de_montaje>`**  
  Desmonta un dispositivo o una partición del sistema de archivos.  
  - **`umount /mnt/usb`**: Desmonta la partición montada en `/mnt/usb`.

- **`blkid`**  
  Muestra información sobre todos los dispositivos de bloques conectados, como identificadores UUID y tipo de sistema de archivos.

- **`fdisk -l`**  
  Lista todas las particiones y detalles de los discos conectados.

### **3. Búsquedas Avanzadas**

- **`find <directorio> -name "<patrón>"`**  
  Busca archivos o directorios por nombre.  
  - **`find /home -name "*.txt"`**: Busca todos los archivos `.txt` en el directorio `/home`.

- **`grep "<patrón>" <archivo>`**  
  Busca texto dentro de un archivo.  
  - **`grep "error" /var/log/syslog`**: Busca la palabra "error" en el archivo `/var/log/syslog`.

- **`locate <archivo>`**  
  Encuentra archivos en el sistema utilizando una base de datos actualizada.  
  - **`locate archivo.txt`**: Busca rápidamente `archivo.txt` en todo el sistema.

### **4. Administración de Procesos y Servicios**

- **`ps aux`**  
  Muestra todos los procesos en ejecución junto con sus detalles.

- **`top`**  
  Muestra en tiempo real los procesos más activos en el sistema.

- **`kill <PID>`**  
  Termina un proceso por su ID de proceso (PID).  
  - **`kill -9 <PID>`**: Fuerza la terminación de un proceso.

- **`service <servicio> start|stop|restart|status`**  
  Administra servicios del sistema.  
  - **`service apache2 start`**: Inicia el servicio de Apache.  
  - **`service ssh status`**: Verifica el estado del servicio SSH.

### **5. Gestión de Usuarios y Permisos**

- **`adduser <nombre_usuario>`**  
  Crea un nuevo usuario en el sistema.

- **`deluser <nombre_usuario>`**  
  Elimina un usuario del sistema.

- **`passwd <nombre_usuario>`**  
  Cambia la contraseña de un usuario.

- **`chmod <permisos> <archivo>`**  
  Cambia los permisos de un archivo o directorio.  
  - **`chmod 755 script.sh`**: Otorga permisos de lectura y ejecución a todos, y permisos de escritura al propietario.

- **`chown <propietario>:<grupo> <archivo>`**  
  Cambia el propietario y el grupo de un archivo o directorio.

### **6. Administración del Sistema**

- **`apt update`**  
  Actualiza la lista de paquetes disponibles en los repositorios.

- **`apt upgrade`**  
  Actualiza todos los paquetes instalados a sus últimas versiones disponibles.

- **`apt install <paquete>`**  
  Instala un nuevo paquete desde los repositorios de APT.  
  - **`apt install nmap`**: Instala la herramienta `nmap`.

- **`apt remove <paquete>`**  
  Elimina un paquete instalado del sistema.  
  - **`apt remove nmap`**: Elimina la herramienta `nmap`.

### **7. Red y Conexiones**

- **`ifconfig`**  
  Muestra la configuración de todas las interfaces de red (requiere privilegios de administrador).

- **`ping <dominio/IP>`**  
  Envía paquetes ICMP a un host para verificar la conectividad de red.  
  - **`ping google.com`**: Verifica la conectividad con Google.

- **`netstat -tuln`**  
  Muestra todas las conexiones de red activas y puertos de escucha.

- **`ssh <usuario>@<host>`**  
  Inicia una sesión SSH en un host remoto.  
  - **`ssh user@192.168.1.100`**: Conecta al usuario `user` en el host `192.168.1.100`.

### **8. Compresión y Descompresión de Archivos**

- **`tar -cvf archivo.tar <directorio>`**  
  Crea un archivo comprimido `.tar` del directorio especificado.

- **`tar -xvf archivo.tar`**  
  Extrae el contenido de un archivo comprimido `.tar`.

- **`gzip <archivo>`**  
  Comprime un archivo usando `gzip`.

- **`gunzip <archivo.gz>`**  
  Descomprime un archivo `.gz`.



///////////////////////////////////////////////////////////////////




### **Laboratorio de Administración de Kali Linux desde la Terminal**

En grupos de dos  o tres integrantes realizar:

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

---
