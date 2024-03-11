# Programacion4Quiz1
El sitio web final esta publicado en: https://dulcet-blancmange-2f30bd.netlify.app/

Para poder usar Bootstrap :

Una vez creado y clonado el repositorio se hicieron las siguientes configuraciones en el proyecto:

Se instala Node.js desde la página oficial: [Node.js](https://nodejs.org/en)

Nota: El instalador también lleva el gestor de paquetes Node.js (npm), por lo que no necesitamos instalar el npm por separado.

Para comprobar la instalación, ponemos lo siguientes comandos en la línea de comandos y deberíamos poder ver las versiones:

node -v 
npm -v
1. Abrimos el proyecto que clonamos para iniciar el proyecto con npm.
2. Abrimos la terminal y nos aseguramos de que esté en la ruta de nuestro proyecto.
3. Escribimos el siguiente comando para configurar nuestro proyecto con npm: npm init -y
4. Si todo salió bien, el comando anterior creó un archivo package.json  en la ruta el proyecto.
5. Ahora se instala Bootstrap con el siguiente comando en la terminal: npm i bootstrap@5.3.3 
    
    Nota: la versión se tomó de la página oficial de Bootstrap: [Bootstrap](https://getbootstrap.com/)
    
6. Si todo salió bien con las instalación de Bootstrap, nos tuvo que crear una carpeta node_modules y un archivo package-lock.json
7. Para poder subir los cambios de la configuración anterior al repositorio, se creó un archivo en la raíz de nuestro proyecto llamado .gitignore. Lo que haremos es ignorar la carpeta node_modules para que no la agregue a los cambios, porque contiene muchos archivos y es lento para subir. En el archivo creado simplemente pondremos: /node_modules 
    


Una vez que tenemos lista la instalacion de Bootstrap , se siguen las siguientes instrucciones para crear nuestro proyecto:

Diseña y desarrolla un sitio web de 3 páginas siguiendo las especificaciones dadas:

Página de Landing:
•	Crea una página de inicio que presente una descripción general de una página de servicio, con un encabezado atractivo y llamativo relacionado con Permisos de Construcción Municipales (como una Agencia asesora o de servicios, no involucre a ninguna Municipalidad).
•	Incluye un llamado a la acción que permita descargar un formulario oficial o acceder a la documentación oficial del formulario en línea para solicitar el servicio.

Página de Explicación:
•	Diseña una página detallada que explique el proceso del servicio ofrecido.
•	Divide la página en secciones con títulos descriptivos.
•	Utiliza imágenes, videos, componentes y documentación (utilice chatgpt para generar textos relacionados de relleno) para enriquecer el contenido.
•	Asegúrate de que el diseño sea atractivo y fácil de entender utilizando las clases de Bootstrap para el estilo.
•	Este formulario debe tener un call to action al formulario web y un link al formulario web.

Formulario Web:
•	Crea un formulario web donde los usuarios puedan completar un permiso de construcción u otro formulario relacionado con el servicio ofrecido.
•	Utiliza componentes de formularios de Bootstrap para diseñar y estructurar el formulario de manera efectiva.
•	Implementa validación del formulario, utilizando las funcionalidades de Bootstrap o JavaScript.

Con base a las instrucciones desarollamos las páginas:

 index.html para el landing.
 service_offered.html para la explicativa.
 form .html para el formulario web.

 Recordemos que utilizamos Bootstrap , así que investigamos el sistema layout de Bootstrap.
 Un resumen de lo que entendimos:

 Bootstrap  trap es una herramienta útil para el diseño de páginas web. Brinda formatos para botones, formularios, alertas, entre otros. Además, su sistema hace que sea fácil adaptar las pantallas de nuestro sitio web en diferentes dispositivos. Para esto, debemos entender el sistema de contenedores filas, columnas y puntos de interrupción.

Contenedores: 
Son los que envuelven, rellenan y alinean el contenido. Básicamente van a contener las filas y columnas que se establezcan.

Filas: 
Son las que envuelven las columnas. Es importante saber que las filas cuentan con hasta 12 columnas.

Columnas: 
Son las que envuelven el contenido. Para las columnas podemos establecer diferentes tamaños, es decir, una fila puede tener 1 columna que abarque toda la fila, o podemos tener 3 columnas que abarquen toda esa misma fila. Sino les damos un tamaño en específico, ellas adoptan el tamaño por defecto, quedando todas del mismo tamaño.
Si queremos establecer los tamaños, como máximo podemos tener 12 columnas. En caso de necesitar menos, se pueden ajustar, para que la suma de ellas sea 12, por ejemplo: 2 columnas, pero una con tamaño de 8 y otra de 4. 

Nota: Las columnas pueden envolver una fila y dentro de esta fila, volver a hacer la lógica de las columnas. 

Puntos de interrupción: 
Los puntos de interrupción son para hacer que, dependiendo del tamaño del dispositivo, se vea o acomode el contenido de la página, de forma que sea más atractiva para el usuario.
Puntos de interrupción: sm, md, lg, xl, xxl. Cada uno de ellos cuenta con dimensiones, por lo que se podría decir, que representan un tamaño de dispositivo. Con estas dimensiones, se modifican las columnas para adaptarse a los diferentes dispositivos. Si tengo 2 columnas, una de 6 y otra de 6, pero quiero que en un dispositivo md, las 2 columnas me abarquen todo el ancho de la pantalla cada una, podemos hacer col-md-12 en cada columna. De esta forma cuando la pantalla tenga las dimensiones de md, se verá 1 columna con todo el ancho de la pantalla y no 2 columnas por fila.

Gracias a esta investigación, hicimos las 3 páginas adaptables a los diferentes dispositivos, esto para mejor visualización del usario.



Una vez finalizado el proyecto, investigamos cómo subirlo a [Netifly](https://app.netlify.com/)
1. Debemos crearnos una cuenta, ya sea con google, GitHub, o hay varias formas de acceder.
2. Simplemente se sube la carpeta del proyecto a la app y este nos genera un dominio para poder acceder desde cualquier lugar.
Nota: Tambien está la posibilidad de enlazarlo a GitHub, y poder escoger la rama que queremos "desplegar". De esta forma cada vez que subamos cambios a Git, en la rama que escogimos en Netlify, se van a ver reflejados los cambios.



##