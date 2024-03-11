# Programacion4Quiz1
El sitio web final esta publicado en: https://dulcet-blancmange-2f30bd.netlify.app/

Para poder usar boostrap:

Una vez creado y clonado el repositorio se hicieron las siguientes configuraciones en el proyecto:

Se instala Node.js desde la página oficial: 

[Node.js](https://nodejs.org/en)

Nota: El instalador también lleva el gestor de paquetes Node.js (npm), por lo que no necesitamos instalar el npm por separado.

Para comprobar la instalación, ponemos lo siguientes comandos en la línea de comandos y deberíamos poder ver las versiones:

node -v 
npm -v
1. Abrimos el proyecto que clonamos para iniciar el proyecto con npm.
2. Abrimos la terminal y nos aseguramos de que esté en la ruta de nuestro proyecto.
3. Escribimos el siguiente comando para configurar nuestro proyecto con npm: npm init -y
4. Si todo salió bien, el comando anterior creó un archivo package.json  en la ruta el proyecto.
5. Ahora se instala Bootstrap con el siguiente comando en la terminal: npm i bootstrap@5.3.3 
    
    Nota: la versión se tomó de la página oficial de Bootstrap:
    
    [Bootstrap](https://getbootstrap.com/)
    
6. Si todo salió bien con las instalación de Bootstrap, nos tuvo que crear una carpeta node_modules y un archivo package-lock.json
7. Para poder subir los cambios de la configuración anterior al repositorio, se creó un archivo en la raíz de nuestro proyecto llamado .gitignore. Lo que haremos es ignorar la carpeta node_modules para que no la agregue a los cambios, porque contiene muchos archivos y es lento para subir. En el archivo creado simplemente pondremos: /node_modules 
    
##