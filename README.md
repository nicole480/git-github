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
