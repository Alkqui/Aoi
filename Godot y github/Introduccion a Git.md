
algunos comandos basicos

ls - En lista los directorios y archivos
pwd  - ver en que ruta de nuestro sistemas esta pocisionado la terminal

es una herramienta que trabaja con el sistema operativo, asi que basicamente se trabaja como si fuera una consola

en git existen *3 estados* , [[Working directory]], [[staging area]], [[repository]]
 
## Cabe resaltar que los comandos no tiene que llegar el guion bajo, son 2 palabras.

#git_init - sirve para crear un proyecto nuevo, o subir uno para utilizar git
#git_add - para poder pasar los archivos del [[Working directory]] al [[staging area]]
#gid_status - estado o ubicacion de los archivos dentro de los 3 estados
#git_commit - pasar los archivos desde el [[staging area]] al [[repository]] solo para crear una 
primera version
#git_push - para subirlo a un repositorio remoto, como el [[github]]
#git_pull - traerte los cambios que han hecho los otros desarrolladores desde [[github]]
#git_clone - traer una copia desde el servidor central, donde se encuentre el proecto, hasta tu computadora
git config --global user.email -- le podemos dar un email de quien esta haciendo los cambios
git config --global user.name -- el nombre del usuario que ha hecho los cambios
#git_log - Para ver todos los commits que hemos creado
#git_restore -- - revierte los cambios de los archivos
#git_diff puedo ver los cambios o diferencias entre los archivos del [[staging area ]] y el [[Working directory]]
## Pequeño tutorial

he creado una carpeta y creado 2 archivos, uno javascript y otro html. ahora sobre la carpeta con click derecho, la abro con el git bash.

tambien se puede hacer desde la consola, entrando a la carpeta del proyecto, y usando #git_init 

al  momento de usar el comando, podemos observar que se ha creado una carpeta dentro del proyecto llamada .git

ahora uso el comando #gid_status 
![[Pasted image 20250705123317.png]]
y podemos ver que los 2 archivos estan *flotando* es decir, estan dentro del [[Working directory]] pero no dentro del [[staging area]]

y entonces los añadimos con  #git_add 
![[Pasted image 20250705123409.png]]

y ahora usamos #git_commit 

nos pide escribir un  mensaje, creo que pones primero la I, porque la consola es bin, y luego de escribir el mensaje, le das a escape, y escribes :qw 

y ahora git le asigna un id a cada archivo
![[Pasted image 20250705124711.png]]
y ahora usamos #git_log 
![[Pasted image 20250705124741.png]]

Ahora todos los archivos estan dentro del [[staging area]] y queda vacio el [[Working directory]]

Ahora he hecho un cambio dentro del archivo html y usado #gid_status 
![[Pasted image 20250705125056.png]]

y entonces puedo revertir los cambios dentro del archivo a la version que tengo dentro del [[staging area]] con  #git_restore y el nombre del archivo

y ahora su vuelvo a cambiar el archivo index.  y uso el comando git diff puedo ver los cambios hecho en el proyecto, y si uso git diff nombre puedo ver los cambios de solo ese archivo
![[Pasted image 20250705125825.png]]

 