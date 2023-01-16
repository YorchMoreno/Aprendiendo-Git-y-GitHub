### PROCESO PARA MANEJO DE GIT Y GIT HUB

[![Imagen tomada de: https://www.google.com/url?sa=i&url=https%3A%2F%2Fvishnuvarshan14fe.medium.com%2Fgit-and-github-essentials-3d144ddbfa88&psig=AOvVaw3hwsHYL6QQ2GLYSR6YOJUW&ust=1673976075760000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCJiluobOzPwCFQAAAAAdAAAAABAD](https://miro.medium.com/max/882/1*D5zGIGFZoEO4uCTriOj4xg.jpeg "Imagen tomada de: https://www.google.com/url?sa=i&url=https%3A%2F%2Fvishnuvarshan14fe.medium.com%2Fgit-and-github-essentials-3d144ddbfa88&psig=AOvVaw3hwsHYL6QQ2GLYSR6YOJUW&ust=1673976075760000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCJiluobOzPwCFQAAAAAdAAAAABAD")](http://https://www.google.com/url?sa=i&url=https%3A%2F%2Fvishnuvarshan14fe.medium.com%2Fgit-and-github-essentials-3d144ddbfa88&psig=AOvVaw3hwsHYL6QQ2GLYSR6YOJUW&ust=1673976075760000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCJiluobOzPwCFQAAAAAdAAAAABAD "Imagen tomada de: https://www.google.com/url?sa=i&url=https%3A%2F%2Fvishnuvarshan14fe.medium.com%2Fgit-and-github-essentials-3d144ddbfa88&psig=AOvVaw3hwsHYL6QQ2GLYSR6YOJUW&ust=1673976075760000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCJiluobOzPwCFQAAAAAdAAAAABAD")
- **GIT:** Sistema de control de versiones que nos permite trabajar de manera colaborativa
[Pagina para descargar GIT](http://https://git-scm.com/download/win "Pagina para descargar GIT")

[![imagen tomada de: https://www.google.com/url?sa=i&url=https%3A%2F%2Fdev.to%2Fcesar_vargas%2Finstalando-git-en-windows-4178&psig=AOvVaw14fd68VZlYpeQRm8kbytL7&ust=1673976139959000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCKj3xKHNzPwCFQAAAAAdAAAAABAV](https://res.cloudinary.com/practicaldev/image/fetch/s--DkkSs3E1--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/s66ilmypzt6m9jymkbpa.jpg "imagen tomada de: https://www.google.com/url?sa=i&url=https%3A%2F%2Fdev.to%2Fcesar_vargas%2Finstalando-git-en-windows-4178&psig=AOvVaw14fd68VZlYpeQRm8kbytL7&ust=1673976139959000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCKj3xKHNzPwCFQAAAAAdAAAAABAV")](http://https://www.google.com/url?sa=i&url=https%3A%2F%2Fdev.to%2Fcesar_vargas%2Finstalando-git-en-windows-4178&psig=AOvVaw14fd68VZlYpeQRm8kbytL7&ust=1673976139959000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCKj3xKHNzPwCFQAAAAAdAAAAABAV "imagen tomada de: https://www.google.com/url?sa=i&url=https%3A%2F%2Fdev.to%2Fcesar_vargas%2Finstalando-git-en-windows-4178&psig=AOvVaw14fd68VZlYpeQRm8kbytL7&ust=1673976139959000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCKj3xKHNzPwCFQAAAAAdAAAAABAV")
- **COMANDOS DE VERIFICACION DE INSTALACION PARA GIT DESDE CMD**
1. Abrimos el CMD de nuestro equipo y escribimos git para instalarlo en la maquina
- **CONFIGURACION DE GIT**
1. Abre el CMD de GIT (click derecho en el escritorio - git bash)
2. Escribe el comando *git config --global user.name (nombre de usuario)*
3. Verifica tu registro con el comando *git config user.name*
4. Ahora registra tu correo con el comando *git config --global user.email (correo electronico)*
5. Verifica tu registro de correo con el comando *git config user.email*
**NOTA:** El repositorio es el mismo proyecto

- **CREANDO REPOSITORIOS EN GIT**
1. Buscamos la direccion de nuestro proyecto den el equipo (el proyecto ya debe estar creado)

**COMANDOS**
(dentro de la consola CMD de GIT abierta desde la carpeta de nuestro poyecto)
1. *git init* (crear nuevo repositorio)
2. *git status* (ver estado del repositorio)
3. *git add .* (agregar todos los archivos que esten dentro de la carpeta de nuestro proyecto)
4. *git commit -m* "(nombre de la modificacion(ejemplo: "primer arreglo"))
**NOTA:** Al guardar el repositorio, se cierra la version que se ha modificado hasta el momento

*git rm --cached* (nombre del repositorio)
este comando es para regresar al anterior commit -m, se usa cuando queremos volver a la anterior modificacion de nuestro proyecto
**NOTA:** gitignore es utilizado para cuando hay archivos con estensiones multimedia que no queremos que se guarden dentro de nuestro repositorio de GIT, la manera de usar es sencilla, primero creamos otro archivo dentro de nuestro proyecto y lo guardamos como .gitignore, dentro de ese archivo colocamos las extensiones que no queremos que se suban a GIT, por ejemplo:

**.mp3* (al anotar este comando dentro del archivo .gitignore de nuestro proyecto, todos los archicos que estes dentro de la carpeta de nuestro proyecto con extension .mp3 no se van a subir a GIT)

- **COMANDO DE SALTO DE TIEMPO**

Esto lo que hace es basicamente devolvernos a cualquier modificacion que hayamos hecho dentro de nuestro editor de texto y guardado en GIT con el comando *git commit -m*
1. Abrimos nuestro Git Bash de nuestro proyecto
2. Vemos los git commit existentes con el comando *git log*
3. Vemos la informacion mas especifica de los git commit existentes con el comando *git log --oneline*
4. Nos devolvemos al git commit que deseemos con el comando *git checkout (nombre del git commit)*
**NOTA:** Al hacer este salto de tiempo, las modificaciones que se hayan hecho a partir del mismo hacia adelante desaparecen
- **RAMAS EN GIT**
Estas son utilizadas por lo general para cuando se emplean trabajos en colaboracion con mas personas, lo que se hace es que se crean ramas o copias del proyecto original y cada integrante puede trabajar enciama de una rama sin afectar la original
1. para ver cuantas ramas hay dentro de GIT en nuestro CMD de GIT de nuestro proyecto codificamos *git branch*
por lo general solo te aparecera una rama llamada **master**
2. para cambiar de ramas dentro de nuestro proyecto usamos el comando *git checkout (nombre de la rama)*

**como crear una rama**

1. comando *git checkout -b (nombre de la rama que se va a crear)*

**NOTA:** Cuando un equipo de trabajo de divide las tareas, estas ramas sirven para que cada uno trabaje en su propia rama sin afectar el proyecto principal, esto genera que dicho proyecto este fragmentado o dividido por el numero de ramas que existan, por ende, hay que unir todo en una rama principal

Para hacer esta union se usa el comando *git merge (nombre de la rama a la cual se quiere unir la rama actual)*

Para eliminar una rama se usa el comando *git branch -d (nombre de la rama que se desea eliminar)*
