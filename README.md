#Dia 1
##¿Qué es git?
Git es un sistema de control de Versiones Distribuido(VCS), esto quiere decir
que se puede trabajar en grupo.
Nos permite guardar archivos y las versiones de estos a lo largo del tiempo
de manera local
##¿Cómo nació git?
Git nació en 2005 cuando Linus Torvalds, creador del kernel de Linux,
 necesitó una nueva herramienta para gestionar los cambios en el código 
del proyecto Linux. Antes utilizaban un sistema llamado BitKeeper,
 que era un software propietario que les permitía trabajar gratis,
 pero tras un conflicto con la empresa que lo desarrollaba,
 dejaron de tener acceso a él. Como solución,
 Linus decidió crear su propio sistema de control de versiones desde cero,
 diseñado para ser rápido, seguro y permitir que muchos desarrolladores
 trabajaran al mismo tiempo. Así surgió Git, que con el paso de los años se
 convirtió en el sistema de control de versiones más utilizado en el mundo del
 desarrollo de software.
##¿Cómo instalar git?
Para instalar git, se tiene que ir a la pagina web de git, y seguir los 
pasos de instalacion recomendados y luego para verifivar la correcta instalacion
se escribe git --version en la terminal
##Configuraciones básicas
- git config --global user.name "Tu nombre"
- git config --global user.email "tu@correo.com"
- git config --global core.autocrlf true
##Archivos que todo repositorio deberia tener
- README.md
- .gitignore
#Día 2-States y commits
##Los estados de git
###Directorio de trabajo(modificado)
Tu carpeta local.Estás escribiendo código, pero Git aún no lo tiene "asegurado".
###Stage Area(preparado)
EL area de espera.Le dices a Git: "Esto es lo que quiero guardar".
###Repositorio local(confirmado)
El  historial.Tus cambios ya tienen un ID(hash) y son parte de la historia.
![flujo de git] (captura.png)
##Directorio de trabajo(modificado)
Este es tu carpeta común, con la diferencia que GIT observa tus
archivos, y los cataloga en:
Untracked: Es decir sin seguimiento, que lo ve pero no tiene una
version antigua de este archivo, sucede cuando este es creado.
Modified: Es cuando GIT ya tiene una version previa del archivo y lo
modificaste, eliminaste o cambiaste de nombre.
Cualquier archivo que no este en el .gitignore pasa automaticamente a
uno de estos estados dependiendo que hayas hecho.
 - El comando git log- oneline sirve para mostrar el commit resumido
  -EL comando git restore <archivo>, sirve para volver el archivo a su estado original,
  Esto borra fisicamente lo que escribimos
  - Si queremos que el archivo que creamos git lo ignore, creamos el archivo .gitignore 
y dentro escribimos los nombres de los archivos a ignorar
##Stage area(Preparado)
Permite seleccionar qué archivos modificados se incluirán en el siguiente commit(guardado)
y cuáles no.
Para traer un archivo al stage area se debe realizar lo siguiente:
-git add<archivo>: Agrega el archivo <archivo>, lo hace uno por uno
- git add. agrega todos los archivos observados por git
Si quieres sacar un archivo del stage area para volver al estado anterior:
git restore --staged <archivo>
##Repositorio Local(confirmado)
Esta es la ultima fase, aqui es donde le decimos al repositorio que cree
el punto de guardado para que todos los cambios que estan en staged
pasen a ser parte del historial
git commit -m "mensaje"
- git reset --soft Head ~1 es para deshacer el ultimo commit(usarlo con precaución)

