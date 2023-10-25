0. su betty
   a. <su> switch user
   b. <user name>
1. whoami
   a. print the current user
2. Groups
   a.Print the current groups
3. Chown betty hello
   a. Cambia el propietario del archivo hello
   b. <chown> change own
   c. <betty> name new own
   d. <hello> file name
6. Chmod 754 hello
   a. Se cambian los permisos al archivo
   b.  <chmod> cambiar los permisos de un archivo
   c. 7 (rwx) -> Lectura, escritura y ejecución.
   d. 5 (r-x) -> Lectura y ejecución.
   e. 4 (r--) -> Solo lectura.
   f.<hello> nombre del archivo
 7. Chmod 751 hello
   a. Se cambian los permisos al archivo
   b.  <chmod> cambiar los permisos de un archivo
   c. 7 (rwx) -> Lectura, escritura y ejecución.
   d. 5 (r-x) -> Lectura y ejecución.
   e. 1 (--x) -> Solo ejecución.
   f. <hello> nombre del archivo
8. Chmod 007 hello
   a. Se cambian los permisos al archivo
   b. establece permisos nulos para el propietario, el grupo
9. Chmod 753 hello
   a. Cambia los permisos del archivo hello
   b. 7 (rwx) permite lectura, escritura y ejecución al propietario.
   c. 5 (r-x) permite lectura y ejecución al grupo.
   d. 3 (---) deniega todos los permisos a otros usuarios.
10. Chmod --reference=olleh hello
    a. Este comando intenta copiar los permisos del archivo olleh (si existe) al archivo hello.
11. Chmod 755 ./*
    a. Cambia los permisos de todos los archivos y directorios en el directorio actual
12. mkdir -m 751 my_dir
    a. Crea un directorio llamado my_dir y establece permisos 751 en él
    b. <-m> indica que se establecerán permisos específicos
    c. <755 > permisos asignados
    d.  <my_dir> nombre del archivo
13. sudo chgrp school hello
    a. <sudo> Ejecuta con permisos de super usuario
    b. <chgrp> cambia el grupo propietario a school
    c. <hello> archivo
14. find . | xargs sudo chown vincent:staff
    a. <find .>Encuentra todos los archivos del directorio actual
    b. <|> pipe une dos operacione
    c. <xargs> Toma la lista de archivos y directorios encontrados por find y la pasa como argumentos al comando que sigue.
    d. <Chown> Cambia el propietario de los archivos
    e. <vincent:staff> nuevo propietario:grupo propietario
15. sudo chown -h vincent:staff _hello
    a. <sudo> Ejecuta con permisos de super usuario
    b. <chown> cambio del propietario
    c. <-h> Solo afecta al enlace simbolico y no a los directorios que apunta
    d. <vincent:staff> nuevo propietario:grupo propietario
    e. <_hello> enlace simbolico
16. sudo chown --from=guillaume vincent hello
    a. <sudo> Ejecuta con permisos de super usuario
    b. <chown> cambio del propietario
    c. <--from=guillaume> condicional de que solo cambia el propietario del archivo si el anterior propietario es guillaume
    d. <vincent> nuevo propietario
    e.<hello> archivo