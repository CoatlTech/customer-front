# Angular CRUD

**Content**   
1. [Como contribuir con este proyecto](#como-contribuir-con-este-proyecto)
2. [Como empezar a usar la aplicación](#como-empezar)
3. [How contribute to this project](#how-contribute-to-this-project)
4. [Getting Started](#getting-started)

## Como contribuir con este proyecto. 
1. Primero, necesitas hacer un fork del repositorio al que deseas contribuir. Esto creará una copia del repositorio en tu cuenta de GitHub. Puedes hacer un fork de un repositorio haciendo clic en el botón "Fork" en la esquina superior derecha de la página del repositorio. 

2. A continuación, necesitas clonar tu repositorio bifurcado en tu máquina local. Esto te permitirá trabajar en los archivos del proyecto sin conexión. Puedes clonar tu repositorio bifurcado utilizando el comando git clone con la URL de tu bifurcación.

3. Después de clonar tu repositorio bifurcado, necesitas crear una rama para trabajar en tus cambios. Una rama es una versión separada del código que puedes modificar sin afectar la rama principal. Puedes crear una rama utilizando el comando git branch con el nombre de tu rama.

4. Una vez que hayas creado una rama, necesitas cambiar a ella utilizando el comando git checkout con el nombre de tu rama. Esto hará que tu rama sea la activa y cualquier cambio que hagas se aplicará a ella. 

5. Ahora puedes empezar a trabajar en tus cambios. Puedes editar, agregar o eliminar cualquier archivo en tu rama como desees. Puedes utilizar cualquier editor de código o IDE que prefieras. 

6. Después de hacer tus cambios, necesitas hacer commit de ellos en tu rama. 

7. A continuación, necesitas enviar tus cambios a tu repositorio bifurcado en GitHub. Esto subirá tu rama y sus commits a tu repositorio en línea. Puedes enviar tus cambios utilizando el comando git push con el nombre de tu remoto (normalmente origin) y el nombre de tu rama.

8. Por último, necesitas crear una solicitud de extracción (pull request) desde tu rama al repositorio original del que hiciste la bifurcación. Una solicitud de extracción es una solicitud para que los mantenedores del repositorio original revisen y fusionen tus cambios en su rama principal. Puedes crear una solicitud de extracción haciendo clic en el botón "Pull Request" en la página de tu repositorio bifurcado en GitHub. 

## Como empezar

### Requisitos
1. Instalar [Node.js LTS](https://nodejs.org/es/) (v18.16.0) o superior y [Angular CLI](https://cli.angular.io/) (v13) o superior.
2. Opcional: Clonar e iniciarlizar el backend de la aplicación [customer-back](https://github.com/sotobotero/customer-back), si no se tiene el backend, la aplicación solo cargrá el front pero no tendra conexión a un back.

### Instalación
1. Clonar el repositorio
2. Entrar a la carpeta del proyecto
3. Instalar los paquetes de npm con el comando `npm install`.
4. Ejecutar el comando `ng serve --configuration=production` para un servidor de desarrollo. Navegar a `http://localhost:4200/customers`. 
La aplicación se recargará automáticamente si se cambia alguno de los archivos de origen.

### Variables de Entorno en Angular 2+
Debido a que esta aplicación se ejecuta en un navegador web, no puedes usar variables de entorno en environments/environment.ts, porque este archivo se ejecuta en el lado del servidor, y las variables de entorno no están disponibles en el lado del servidor.

Si deseas usar variables de entorno en environments/environment.prod.ts, necesitas cambiar el enfoque para usar la librería dotenv y el plugin dotenv-webpack para webpack.
