0. echo "Hello, World"
   a. <echo> imprime
   b. <"Hello, World"> texto impreso
1. echo "\"(Ôo)'"
   a. <echo> imprime
   b. <"\> imprime los caracteres literales 
   c. <"(Ôo)'"> caracteres impresos
2. cat /etc/passwd
   a. <cat> muestra el contenido del achivo
   b. </etc/passwd> ubicacion del archivo
3. sudo cat /etc/passwd /etc/hosts
   a. <sudo> super usuario
   b. <cat> muestra el contenido del achivo
   c. </etc/passwd /etc/hosts> las rutas de los archivos
4. tail -n 10 /etc/passwd
   a. <tail> mustra las ultimas lineas de un archivo
   b. <-n 10> se indican el numero de lineas a mostrar
   c. </etc/passwd> ruta del archivo
5. head -n 10 /etc/passwd
   a. <head> muestra las primeras lineas de un archivo
   b. <-n 10> se indican el numero de lineas a mostrar
   c. </etc/passwd> ruta del archivo
6. tail -n +3 iacta | head -n 1
   a. En este caso muestra solo la tercera linea del archivo
   b. <tail> mustra las ultimas lineas de un archivo
   c. <-n 3> se indican el numero de lineas a mostrar
   d. <iacta > ruta del archivo
   e. <|> pipe envia el resultado al siguiente comando
   f. <head> muestra las primeras lineas de un archivo
   g. <-n 1> se indican el numero de lineas a mostrar
7. echo 'Best School' > \\\*\\\\"'\"Best School\"\\'"\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*:\)
   a. Crea un archi llamado <\*\\'"Best School"\'\\*$\?\*\*\*\*\*:)> y escribe <Best School>
   b. \*: Representa un asterisco (*).
   c. \\: Representa una barra invertida ().
   d. \': Representa una comilla simple (').
   e. \": Representa una comilla doble (").
   f. \?: Representa un signo de interrogación (?).
   g. \*: Representa un asterisco (*).
   h. \*: Representa un asterisco (*).
   i. \*: Representa un asterisco (*).
   j. \*: Representa un asterisco (*).
   k. :): Representa la secuencia de caracteres ":)"
8. ls -la > ls_cwd_content
   a. <ls  -la> lista los archivos con formato largo incluyendo ocultos
   b. <>> el resultado anterior lo envia al archivo sobre escribiendo
   c. <ls_cwd_content> archivo
9. tail -n 1 iacta >> iacta
   a. En este caso duplica la ultima line del archivo
   b. <tail> mustra las ultimas lineas de un archivo
   c. <-n 1> se indican el numero de lineas a mostrar
   d. <iacta > ruta del archivo
   e. <>>> el resultado anterior lo envia al archivo sin sobre escribir
   f. <iacta>ruta del archivo
10. sudo find . -type f -name "*.js" -delete
    a. Elimina todos los archivs terminados en .js del archivo actual
    b. <sudo> permiso de super usuario
    c. <find .> encuentra todos los archivos en el directorio actual
    d. <-type f > se buscar archivos regulares (no directorios ni otros tipos de archivos).
    e. <-name "*.js"> se deben buscar archivos cuyo nombre termine con ".js"
    f. <-delete> Elimina los archivos que cumplan con las condiciones
11. find . -type d ! -path . -print | wc -l
    a. En este caso cuenta directorios y sub directorios del actual archivo excluyendo en contar el archiv actual
    b. <find .> encuentra todos los archivos en el directorio actual
    c. <-type d> se buscaran solo directorios
    d. <! -path .> excluye el directotio actual
    e. <-print>imprime la ruta del directorio encontrado
    f. <|>  envia el resultado al siguinete comando
    g. <wc -l> cuenta las lineas
12. ls -t | head -n 10
    a. Mustra las 10 entradas más recientes
    b. <ls -t> lista los archivos y los ordena por fecha de modificacion
    c. <|> pipe envia el resultado al siguiente comando
    d. <head> muestra las primeras lineas de un archivo
    e. <-n 10> se indican el numero de lineas a mostrar
13. sort | uniq -u
    a.  En este caso ordena y elimina las lineas duplicadas
    b. <sort> ordena las lineas de entrada en orden alfabetico
    c. <|> pipe envia el resultado al siguiente comando
    d. <uniq >  elimina las líneas duplicadas consecutivas de la entrada
    e. <-u> muestra las linesa unicas sin duplicados consecutivos
14. grep "root" /etc/passwd
    a. <grep > busca patrones de texto en un archivo y muestra las líneas que coinciden con el patrón especificado
    b. <"root"> patron a buscar
    c. </etc/passwd> ruta del archivo
15. grep -c "bin" /etc/passwd
    a. <grep > busca patrones de texto en un archivo y muestra las líneas que coinciden con el patrón especificado
    b. <-c> cuenta el número de líneas que coinciden con el patrón especificado
    c. <"bin"> patron a buscar
    d. </etc/passwd> ruta del archivo
16. grep -A 3 "root" /etc/passwd
    a. Busca el patron root en el archivo, lo muestra y las tres lineas siguientes
    b. <grep > busca patrones de texto en un archivo y muestra las líneas que coinciden con el patrón especificado
    c. <-A 3> especificar cuántas líneas siguientes a la coincidencia se mostrarán
    d. <"root"> patron a buscar
    e. </etc/passwd> ruta del archivo
17. grep -v "bin" /etc/passwd
    a. Busca y muestra en el archivo todas las lineas que no tienen "bin"
    b. <grep > busca patrones de texto en un archivo y muestra las líneas que coinciden con el patrón especificado
    c. <-v> invierte la busqueda
    d. <"bin"> patron a buscar
    e. </etc/passwd> ruta del archivo
18. grep '^[A-Za-z]' /etc/ssh/sshd_config
    a. <grep > busca patrones de texto en un archivo y muestra las líneas que coinciden con el patrón especificado
    b. <^[A-Za-z]> Indica que debe buscar una linea que inicie con mayuscula o minuscula
    c. </etc/ssh/sshd_config> archivo
19. tr 'A' 'Z' | tr 'c' 'e'
20. tr -d 'c' | tr -d 'C'
21. Rev
22. cut -d ":" -f 1,6 /etc/passwd | sort