1. #!/bin/bash
   a. Se coloca al inicio de un script en unix para identifdicar por el sistema que se debe ejecutar como script
   Pwd
   a. print working directory
2. Ls
   a. Lista los archivos y directotios
3. Cd
   a. Change directori
4. ls -l
   a. Lista los archivos y directorios
   b. <-l> con formato largo  mas detallado
5. ls -lan
   a. Lista los archivos y directorios
   b. <-l> con formato largo <-l> mas detallado
   c. <-a> muestra tambien los archivos ocultos
   d. <n> cambia los nombres de usuario por información númerica
6. mkdir -p /tmp/my_first_directory
   a. Make directoty
   b. -p crea los directorios intermedios si no estan creados
7. mv /tmp/betty /tmp/my_first_directory/
   a. Move
   b. Mueve betty de tmp a my_first_directory
8. rm -f /tmp/my_first_directory/betty
   a. Remove
   b. <-f> forzado elimina el archivo sin pedir confirmacion
9. rm -rf /tmp/my_first_directory
   a. Remove
   b. <-r> recurcive  elimina todos los archivos dentro del directorio
   c. <-f> forzado elimina el archivo sin pedir confirmacion
10. cd -
   a. Change directori
   b. <-> vuelve al directorio en que estaba anteriormente
11. ls -la . .. /boot
   a. Lista los archivos y directorios
   b. <-l>
   c. <-a>
   d. <.> Es el directotio actual
   e. <..> El directorio padre del directorio actual
   f. </boot> es una ubicacion del sistema
12. file /tmp/iamafile
   a. <FILE> determina el tipo de archivo
13. ln -s /bin/ls __ls__
   a. <ln> crea enlaces simbolicos y duros
   b. <-s> indica que se debe crear un enlace simbolico
   c. < /bin/ls> la ubicacion del archivo ejecutable
   d. <__ls__> es el nombre del enlace simbolico
14. cp -n ./*.html ..
   a. <cp> copia archivos
   b.  <-n> --no--clobber no sobre escribe archivos con el mismo nombre y lo copia con otro nombre
   c. </*.html> solo selecciona archivos .html del directorio actual
   d. <..> es el directorio donde se van a copiar en este caso el directorio padre
15. mv [A-Z]* /tmp/u/
   a. <mv> mueve los archivos o cambia el mombre
   b. <[A-Z]*> selecciona los archivos que inician con una letra mayuscula
16. rm -f *~
   a. <Remove>
   b. <-f> forzado elimina el archivo sin pedir confirmacion
   c. <*~> selecciona los archivos que se eliminaran en este caso los que inician con ~
17. mkdir -p welcome/{to/school,}
   a. Make directori
   b. <-p>  crea directorios intermedios
   c. <welcome/{to/school,}> en este caso crea el directorio welcome y dentro crea to y school