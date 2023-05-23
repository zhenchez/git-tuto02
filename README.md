#### La otra otra parte de la documentación está aquí: [2.1-2.3](https://docs.google.com/document/d/1aViOODB5V0rU2c7oV4HQJuFGX32JT8SZhY8r3kmLo5o/edit?usp=sharing "Documentación anterior") 

>2.4 - Entra en este manual de Markdown y haz un resumen de los principales comandos de Git con los que hemos trabajando. Puedes utilizar tablas, imágenes, títulos, enlaces, etc.
>>* **Configurar Git**  
En un principio deberiamos congifurar Git asociando nuestro nombre de usuario y nuestro correo electronico usando las siguientes líneas de comando:  
**git config --global user.name "username"**  
**git config --global user.email "email"**
***
>>* **Iniciamos nuestro repositorio local**  
Para que un directorio de nuestra máquina se convierta en un repositorio local usaremos la siguiente línea de comando:  
**git init "directory"** o bien nos situamos en el direcorio y realizamos un **git init**.
***
>>* **Comprobar el estado de nuestro repositorio**  
Para combrobar los archivos que no están reconocidos, que están modificados o añadidos a la **staging area**. Los podeos ver usando un:  
**git status**
***
>>* **Cambiar archivo de estado**  
>>**1. ADD:** En el caso de que tengamos un archivo no reconocido, deberemos añadirlo a la **staging area** para que el repositorio lo reconozca. Para ello usaremos:  
**git add "archivo"** o bien si queremos añadir todos los archivos de nuestro repositorio usaríamos **git add .**.  
>>  En el caso de haber añadido un archivo que ya no queremos, usaremos:  
**git rm --cached "archivo"**  
>>**2. COMMIT:** Una vez que tengamos los archivos en el **staging area** sería hora de realizar un commit utilizando:  
**git commit -m "(Descripción)"**.
***
>>* **Visualizar todos nuestros commits**  
Para visualizar los commits que hemos realizado podemos utilizar el siguiente comando:  
**git log --all --oneline --graph**
***
>>* **Asociar un repositorio local a uno remoto**  
Hasta ahora estabamos hablando de un repositorio local. Ahora, para asociarlo a un repositorio remoto deberiamos crear uno, ya sea en **GitHub**, **BitBucket** o **GitLab**. Una vez creado habria que asocial el repositorio local al respositorio remoto. Usando las siguientes líneas e código:  
**git remote add origin "enlace de tu repositorio remoto"**  
**git branch -M main**  
**git push -u origin main**  
>> Hecho este paso, podríamos ver que nuestro repositorio está asociado utilizando:  
**git remote -v**
***
>>* **Retroceder a versiones anteriores**  
Siempre que queramos volver a como lo dejamos en un cierto commit, podemos usar:  
**git checkout "hash del commit en cuestión"**  
El hash de un commit lo podemos reuperar utilizando el comando para visualizar todos nuestros commits.
***
>>* **Clonar repositorios**  
Siempre que tengamos el enlace del repositorio a clonar podremos clonarlo sin ningún problema usando:  
**git clone "enlace"**
