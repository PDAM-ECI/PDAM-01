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

![alt text](https://drive.google.com/file/d/0B9J6w04FyNE7bUkwN0R5TEcyTkk/view)

# Reto
Investigue como crear una accion de slide sobre los elementos de la lista, esto con el fin de habilitar un boton de borrar una vez se haga slide sobre el elemento deseado. [Referencia](http://ionicframework.com/docs/api/directive/ionList/)
