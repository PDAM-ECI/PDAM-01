# PDAM-01

Usando la siguiente guía el estudiante podrá entender el funcionamiento de las aplicaciones móviles híbridas. 
En este caso particular se usará el framework de ionic que usa AngularJS para el desarrollo del flujo de la aplicación.

Durante el laboratorio se construira una aplicación sencilla en la que se podra tener una vista de listado de elementos y una vista donde se editará el perfil del usuario.

# Instalación de software
Para comenzar revise en su maquina si los siguientes componentes están instalados, ejecutando desde una consola los siguientes comandos:
* NodeJS: node --version
* npm: npm --version
* ionic: ionic --version

# Creación del prototipo de la aplicación
Para crear un prototipo de una aplicación que puede ser descargado para ser compilado, debe crear una cuenta en [ionic creator](https://creator.ionic.io/app/login). Esta aplicación web es gratuita.
Después de haber creado la cuenta debe ingresar y crear un nuevo proyecto. Al crear el proyecto se le darán 4 opciones, escoja la opcion side menu.
El menu debe contener dos elementos:
* Inicio
* Perfil

En la parte izquierda aparecen todas las vistas que tiene la aplicación, cambie el nombre de la vista Home por Inicio, y el de la vista
Cart por Perfil. Es importante que tambien se ajuste la url "Routing URL" acorde al titulo de la vista, esto servirá de guía cuando se haga la generacion de código.
Dentro de la vista de Inicio deberá estar la lista que contiene elementos "TODO" que el usuario ingresará y seran almacenados localmente, para crear una lista en esta vista, ubique al lado izquierdo en el panel de componentes, el componente de lista. Arrastre este componente a la vista de Inicio. Esto creará una lista con 3 elementos de prueba.
Teniendo la vista de inicio seleccionada, ubique el panel de la derecha en donde se encuentran las propiedades de la vista. En este panel ubique la sección "Right header button". Habilite el botón (enable) y seleccione un icono de su preferencia, este boton aparecera en el header de la vista, este boton servira para que el usuario pueda crear agregar elementos a la lista. 

En la vista de Perfil agregue componentes y ordenelos hasta que quede como en el siguiente ejemplo:

![alt text](http://gabo.com.co/pdam/lab-01-01.png)

Ubique dentro del panel izquierdo la vista de Cloud, cambie el nombre por Edicion. A continuación entre a la vista de perfil y seleccione el boton de cambiar contraseña, en el panel de la derecha ubique la sección de link, dentro del selector seleccione la vista de Edicion. Esto hará que al hacer clic al botón se navegue a la sección deseada.

En la vista de Edicion, agregue los componentes necesarios para que la vista quede como el siguiente ejemplo:

![alt text](http://gabo.com.co/pdam/lab-01-02.png)

Usando el modo preview, revise que la aplicacion haya quedado correctamente creada y que los menus y botones naveguen de manera correcta. Con este modo puede revisar el funcionamiento del prototipo.

# Generación de la aplicación
La herramienta provee la capacidad de crear el codigo necesario y funcional de las vistas creadas en el prototipo. Para usar esta herramienta ubique en la parte superior derecha el icono de Export your App. 

![alt text](http://gabo.com.co/pdam/lab-01-03.png)

Dentro de las varias alternaitvas seleccione el paquete ZIP. Esto generará un archivo descargable con la aplicación funcional.
Descargue y abra el archivo. Entre por linea de comando a una nueva carpeta y ejecute el siguiente comando para inicializar la aplicación de ionic:

```javascript
ionic start pdam_1 sidemenu
```
Esto generara una aplicacion demo, se puede usar esta aplicacion y remplazar los archivos que se descargaron de ionic creator. Remplace los archivos que descargó e incluyalos indicados dentro de la carpeta www del proyecto que se genero en el comando anterior

ejectue el siguiente comando para probar la aplicación en modo explorador

```javascript
ionic serve
```

Para probar la aplicación en un dispositivo real Android. Ejecute el siguiente comando.

```javascript
ionic build android
```

Esto generará un APK que podrá instalar en su dispositivo.

# Reto
* Investigue como instalar el APK en su telefono móvil
* Investigue como adicionar elemenos nuevos al listado de prueba usando AngularJS
* Investigue como crear una accion de slide sobre los elementos de la lista, esto con el fin de habilitar un boton de borrar una vez se haga slide sobre el elemento deseado. [Referencia](http://ionicframework.com/docs/api/directive/ionList/)
