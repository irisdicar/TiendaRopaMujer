# Bienvenidos  a IDC_Craft

# IDC_Craft
Es una aplicacion de venta manualidades realizada con alumino y madera 
  
  
# Información de la aplicación y el equipo
Nombre de la aplicación: IDC_Craft
Cliente: Multiservicios Loa Ardicar C.A
Equipo de desarrollo:
Carlos Dev (desarrollador de Android: mayo de 2018 - junio de 
2019),
Nadia Dev (desarrollador de Android: junio de 2019 - hasta la 
fecha),
Encarnación Dev (desarrollador de backend: mayo de 2016 -
hasta fecha)
Equipo de diseño: Juan Blanco, Cristina Fernández
Gestión: Pedro Gómez (Gerente superior: mayo de 2012 - junio 
de 2016), Antonio López (Gerente superior: julio de 2016 -
hasta la fecha)
URL web: http: // www.idc-craft.com
________________________________________
# Acerca de este archivo
El objetivo de este archivo es proporcionar una descripción general, instrucciones de configuración e información básica del proyecto. Si se unió a este proyecto como parte del equipo de desarrollo, asegúrese de que este archivo esté actualizado.
Nota: cualquier dependencia agregada/modificada a este proyecto que afecte la ejecución del código en este repositorio de git debe enumerarse en este archivo. Todos los desarrolladores deben asegurarse de que las instrucciones mencionadas en este archivo sean suficientes para permitir que un nuevo desarrollador obtenga una copia ejecutable del código más reciente en este repositorio, sin la participación de ninguna otra asistencia humana.
________________________________________
# Software y Hardware requerido
I) Software requerido
1.	Windows
2.	Maven
3.	JDK
4.	Http Server
5.	MySQL and MySQL drivers
II) Hardware requerido
1.	Minimum 8 GB RAM
2.	Minimum 12 GB Available Disk Space
3.	Wifi Availablility

# Especificaciones técnicas de Proyecto
* Este proyecto esta elaborado en el elengauje de programacion HTML y utiliza PHP como Back-end
* El código angular se compila primero usando comandos 
angular-cli, 
 luego la salida se mueve al directorio www de cordova.
Después de lo cual,
 el comando cordova build genera la salida final de Android 
/ iOS. * La API es proporcionada por el cliente
* El diseño de referencia es del
 equipo de diseño de XYZ Company Pvt Ltd Mumbai 

________________________________________
Setup Instructions
As mentioned earlier , this is a cordova-angular project,
The below mentioned steps may vary significantly across various operating systems, please follow them accordingly.
These instructions are aimed at a developer who has been added to the project team, after the project development has already been initiated,
Therefore the aim is to get the code from the git repository to run on the developer's system, so as to allow him / her to continue with further development.
________________________________________
Clone the repository from GitLab :
git clone git@gitserver.abccompanygit.com:root/rocket.git
Change current working directory to Project directory
cd Rocket
( This is the cordova as well as the angular root folder. )
Checking out the latest development branch
As of writing this guide the main branch used for development is : develop
To switch to this branch run :
git checkout develop
Installing dependencies
This project requires cordova for running, You can install it by referring to the official cordova page : [https://cordova.apache.org/]
The cordova version used at the time of writing this file is : 8.1.2 You can check the installed version using cordova -v
The config.xml file contains the list of all cordova plugins and platforms used for this project. Please ensure this file is updated incase any plugin is added / removed.
Please follow below steps for installation :
Install Angular and Cordova NPM Dependencies
npm i
Next install cordova platforms and plugins
cordova prepare
Incase you get errors as : Current working directory is not a Cordova-based project.
The www folder used by cordova cli to detect a cordova project might be missing Simply make an empty www folder via file manager or via commandline as :
mkdir www
Install cordova android platform
cordova platform add android
________________________________________
Start the http and mysql xampp server :
xampp http start
xampp mysql start
sudo service kurento-media-server-6.0 start
________________________________________
Note for future developers
Home is an addon module which adds search by name functionality to the core code The files in the above directory when included in the index file overwrites methods, variables, css in the core code and manipulates the DOM at runtime by adding / removing elements. Thus the entire search logic is separated and can be included on demand, This is the first attempt of adding additional features as modules Future features if any should also be done in the same way, The core code should only be modified for bug fixes or core updates Any new feature either core or customer specific should be implemented as a pluggable module in the /project_directory/src/main/resources/static/addons/ directory

