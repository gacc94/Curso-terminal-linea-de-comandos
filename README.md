
# Curso Terminal linea de comandos
***
### Imagen de los comandos
![Comandos](/src/plantilla%20Hoja%20comandos%20.jpg )
### Comando
listar :

`ls` long `ls -l` all/ocultos: `ls -la` reverse `ls -lr`

change directory `cd`

Instalar TREE - Arbolde directorios  `sudo apt install tree`
directorios por niveles `tree -L #(1,2,3)`

Crear directorio `mkdir miCarpeta`

Crear Archivo  `touch miArchivo1 miArchivo2`

Copiar Archivo `cp file1 file2`

Mover archico o directorio `mv file1 router` o `mv miDirectorio1 miDirectorio2`
se pued mover archivo a directorios anteriores `mv file1 ../` 
renombrar archivo `mv file1 file_rename`  


Eliminar o remover archivo  `rm file`
Eliminar directorio forzado `rm -rf miDirectorio`
Eliminar directorio interactivo `rm -ri miDirectorio`

Cabecera de un archivo de texto (-n = numeros filas)`head miArchivo -n 5`

Ulimas filas de archivo de texto(-n = numeros de filas) `tail miArchivo -n 5`

Explorar archivo de textp `less miArchivo`

Abrir archivo con editor de codigo predeterminadp `xdg-open miArchivo`

Comando para saber el tipo o descripcion de un comando `type archivo o directorio`

Crear un alias para ejecutar comandos predeterminados `alias l = "ls -lh"`

Obtener el manual de un comando `man cd`

informacion de un comando `info mkdir`

informacion abreviada de un comando `whatis mkdir`
***
## Wildcards
Buscar por coincidencias todos `ls *.txt` por inicio `ls file*` 
que tenga 1 caracter al final (entre mas interrogacion mas caracteres) `ls file?`
por mayusculas `ls [[:upper:]]*`

***
## File Descriptor / Redirreciones

### Pipe Operator
emprimir la salida en la terminal `echo "Hola Platzi "`
concatenar archivos `cat miArchivo1 miArchivo2`

rediregir la salida de un comando hacia un archivo 
`cowsay "Hola amigo " | cat | tee cat.txt` 

Encadenar comandos con ampersan & `ls & date`

Crear carpeta y mover hacia la carpeta creada`mkdir test && cd test`

### Manejo de Permisos 

### Modificando permisos terminal

comando `chmod 755 miArchivo`

comando para saber quien soy en la temrinal `whoami`

cambiar usuario root `su root`

## Comandos de busueda 

Buscar localizacion de un programa `which code` (vscode)

Buscar desde una carpeta especifico (-d=directory)`find ./ -type d -name Documents
`
## GREP
buscar ´por coincidencias en archivp csv `grep Towers miArchivo.csv`
case sensitive (-i) `grep -i Towers movies.csv`

## Comandos para RED

sobre nuestra red `ipconfig`
ping a una pagina web `ping www.google.com`

## Comprimir Archivos Tar y Zip
comprimir Tar ` tar -cvf ToCompress.tar ToCompress`

comprimir Tar de manera eficiente `tar -cvzf ToCompress.tar.gz ToCompress`

descomprimir archivo Tar `tar -xzvf miArchivoTar.tar.gz`

Comprimir Zip `zip  -r MiArchivo.zip CarpetaComrprimir`

Descomprimir unzip ` unzip ToCompressInZip.zip  `

### Manejo de Procesos

comando para ver los procesos `ps` eliminar procesos `kill miProceso`
