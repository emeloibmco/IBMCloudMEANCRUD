# IBMCloudMEANCRUD
Hands On para construir aplicación utilizando el Stack MEAN en IBM Cloud

## Índice

* Creación y despliegue de la MEAN Stack App.
* Creación base de datos y enlace con el MEAN Stack App.

##  Introducción
En la siguiente guía puede observar cómo se realiza la creación, el despliegue y la modificación de un Mean
stack, con mongo Db, Express.js, Angular y node.js en IBM Cloud.

##  Creación y despliegue MEAN Stack App

Para realizar la creación del Mean stack, se dirige a la página principal de Cloud IBM en la cual pude acceder
por medio de la siguiente **URL** https://cloud.ibm.com/login/, una vez allí va a iniciar sesión con su cuenta
de IBM Cloud.

<img width="600" alt="1" src="https://user-images.githubusercontent.com/50923637/58988050-6fb58a00-87a6-11e9-9d23-6b0cf0cde805.png">

Una vez le haya dado clic en `log-in`, va a aparecer la siguiente pantalla.

<img width="600" alt="2" src="https://user-images.githubusercontent.com/50923637/58988061-73e1a780-87a6-11e9-9fad-3cab02af432b.png">

Luego de la autenticación de usuario y contraseña, se va a ver la página inicial de IBM Cloud donde puede
verificar los servicios y aplicaciones que tiene creados actualmente, Una vez allí se va a dirigir a el **menú de
hamburguesa** o **menú de navegación** y da clic en él.

<img width="600" alt="3" src="https://user-images.githubusercontent.com/50923637/58988064-7512d480-87a6-11e9-8dd0-b1a30cda7364.png">

Luego de dar clic en el menú de hamburguesa se despliega un panel con varias opciones que ofrece IBM Cloud,
en la cual se dirige hasta el último ítem llamado **Web Apps** y da clic en él.

<img width="600" alt="4" src="https://user-images.githubusercontent.com/50923637/58989374-6da0fa80-87a9-11e9-9376-edd7b6bdeb46.png">

Luego de ingresar a **Web Apps** se despliega la siguiente pantalla en la cual, va a dar clic en la opción **Get
started**, ubicada dentro del cuadro o segmento **Start from the web**.

<img width="600" alt="5" src="https://user-images.githubusercontent.com/50923637/58989376-6ed22780-87a9-11e9-8c10-f803c73f72cf.png">

Luego de dar clic en **Get started** se direcciona a la siguiente pagina la cual da las opciones o las características
con las cuales va a contar el Mean Stack que se quiere crear, en el cual va a seleccionar la opción **MEAN
Stack: Mongo Db, Express.js, Angular, Node j.s**.

<img width="600" alt="6" src="https://user-images.githubusercontent.com/50923637/58989379-70035480-87a9-11e9-8aba-e703afc5cee4.png">

Luego de ingresar podrá ver la siguiente pagina en la cual puede ver que se realizó la selección del MEAN Stack
deseado, da una serie de características con las que cuenta el servicio que anteriormente selecciono, estando en
esta pagina da clic en **Create App** para poder dar inicio a la creación de la aplicación que desea realizar y
desplegar.

<img width="600" alt="7" src="https://user-images.githubusercontent.com/50923637/58989385-71348180-87a9-11e9-8bd7-98367b1d6799.png">

Luego accede a otra pagina en la cual le permite dar el nombre que desea para su aplicación, un tag si lo desea
agregar y a su vez especifica que la aplicación trabaja con la plataforma de Node.js, luego de establecer un
nombre a la aplicación da clic en **Create**.

<img width="600" alt="8" src="https://user-images.githubusercontent.com/50923637/58989729-151e2d00-87aa-11e9-8a0a-26cd2860e6e7.png">

Luego esto tomara un par de segundos para darle acceso a la siguiente página, en la cual le da la opción de
desplegar la aplicación en Cloud, para desplegar la aplicación debe dar clic en la opción **Deploy to Cloud**.

<img width="600" alt="9" src="https://user-images.githubusercontent.com/50923637/58989730-164f5a00-87aa-11e9-8a8e-9f555f639387.png">

Luego de dar clic en **Deploy to Cloud foundry** se despliega una ventana en la cual le da la opción de
seleccionar la región en la cual desea desplegar la aplicacion, memoria que desee provisionarle a la aplicación,
la organización, el espacio y el dominio donde va a estar asignado.

<img width="600" alt="10" src="https://user-images.githubusercontent.com/50923637/58989735-17808700-87aa-11e9-8a86-ed615de3bfd7.png">

`Nota: Tenga en cuenta las condiciones de latencia según su ubicación para así poder seleccionar
la opción de región óptima para usted.`


Luego vera la ventana anteriormente mencionada, en ella seleccionara la memoria deseada, el número de instancias
deseadas, la región, la organización, espacio y el dominio, en esta ventana luego de seleccionar lo deseado
da clic en **Next**.

<img width="600" alt="11" src="https://user-images.githubusercontent.com/50923637/58989915-6fb78900-87aa-11e9-9821-7e7229669339.png">

Luego sale una ventana en la cual **configurara el Toolchain**, le asigna el **nombre deseado**, asigna la **región**
y el **resource group**, después de esto da clic en **Create**.

<img width="600" alt="12" src="https://user-images.githubusercontent.com/50923637/58989917-70501f80-87aa-11e9-9108-a88dc1a4aabc.png">

Luego de haber dado clic en **Create**, se demorará un par de segundos en terminar el proceso, ya cuando el
proceso termina, podrá ver que aparece que ya se configuro las provisiones deseadas para la aplicación, luego
da clic en **View Toolchain**.

<img width="600" alt="13" src="https://user-images.githubusercontent.com/50923637/58989918-71814c80-87aa-11e9-860a-7322ed4c14f0.png">

Luego aparece la siguiente ventana en la cual podrá visualizar las opciones de Think, Code y Deliver, al estar
en esta página deberá acceder **Delivery Pipeline** para verificar que el despliegue de la aplicación se realizó,
está en proceso de despliegue o ver si fallo el despliegue de la aplicación.

<img width="600" alt="14" src="https://user-images.githubusercontent.com/50923637/58989920-72b27980-87aa-11e9-9fdd-f7f9fb974ec9.png">

Luego en la ventana siguiente podrá ver si el despliegue se esta realizando, cuando el **Build stage**, el **Deploy
stage** y el **Healt stage**, cuando estos tres ítems se encuentren en `STAGE PASSED` puede tener certeza que
el despliegue se realizo de forma correcta, en caso de que alguna de las etapas no se despliegue correctamente,
se debe dar clic en el botón de **run stage** para volver a iniciar el proceso de despliegue de la aplicación.

<img width="600" alt="15" src="https://user-images.githubusercontent.com/50923637/58990178-f10f1b80-87aa-11e9-8205-2570082c1aa1.png">

## Creación de bases de datos y enlace con el MEAN Stack App

### Creación base de datos

Luego da clic en el **menú de hamburguesa** para acceder al **Resource list** o **la lista de recursos**.

<img width="600" alt="16" src="https://user-images.githubusercontent.com/50923637/58990183-f2404880-87aa-11e9-9d3b-7c24a95a0333.png">

Luego deberá dar clic en la opción **Resource list** o **lista de recursos**.

<img width="600" alt="17" src="https://user-images.githubusercontent.com/50923637/58990184-f3717580-87aa-11e9-8d86-ba9358b28879.png">

Después se da clic para desplegar el menú de **Apps** existente en el **resource list** o **lista de recursos**, deberá
buscar la aplicación que creo dentro del menos de aplicaciones que se despliega que fueron anteriormente creadas
y debe dar clic en la aplicación en la cual está trabajando en el momento.

<img width="600" alt="18" src="https://user-images.githubusercontent.com/50923637/59036108-4ba08a00-8834-11e9-9fce-55fd71808670.png">

Luego de dar clic en la aplicación, será redireccionado a la siguiente ventana en la cual va a dar clic en la opción
**Add resource** o **Añadir recurso**.

<img width="600" alt="19" src="https://user-images.githubusercontent.com/50923637/59036111-4d6a4d80-8834-11e9-9249-b0defa08852a.png">

Luego se ve una ventana en la cual seleccionará el recurso que desea agregar a la aplicación en este caso dará
clic en la opción **Databases**, luego de ver que esta seleccionada da clic en **Next** o **Siguiente**.

<img width="600" alt="20" src="https://user-images.githubusercontent.com/50923637/59036117-4e9b7a80-8834-11e9-9d56-57d255e9fe6c.png">

Luego en la ventana aparece el recurso que desea agregar, deberá buscar la opción **Databases for MongoDB**,
seleccionará esta opción y da clic en **Next**.

<img width="600" alt="21" src="https://user-images.githubusercontent.com/50923637/59304238-712afa80-8c5d-11e9-9bca-351f14ef97c5.jpg">

Después de eso se realiza el despliegue, en la ventana las opciones deben seleccionar la región, está ya seleccionado
el resource group o grupo de recursos anteriormente asignado luego de eso deberá dar clic en la opción **Create**
o **Crear**.


`Nota: Para poder agregar un recurso a una aplicación se debe tener en cuenta que la cuenta
debe contar con permisos o debe ser una cuenta paga es decir con recursos para poder realizar
esta acción de provisionar recursos.`

<img width="600" alt="22" src="https://user-images.githubusercontent.com/50923637/59304240-72f4be00-8c5d-11e9-9ba8-fdec5691191d.jpg">

Luego este proceso durara un par de minutos, para poder hacer que el recurso quede provisionado en la aplicación.

`Nota: Tener en cuenta que la región seleccionada coincida en cada uno de los campos donde se
requiera para poder establecer conexiones correctas.`

`Nota: El recurso no aparece a la vista de la Aplicación.`

Para poder ver el recurso agregado se da clic en **Add resource** o **Añadir recurso** nuevamente.


<img width="600" alt="19" src="https://user-images.githubusercontent.com/50923637/59036111-4d6a4d80-8834-11e9-9249-b0defa08852a.png">

En la ventana que se genera se debe ir hasta la parte de abajo hasta el punto donde dice **Existing services** o
**Servicios existentes**, se selecciona y luego se da clic en **Next** o **Siguiente**.

<img width="600" alt="23" src="https://user-images.githubusercontent.com/50923637/59036620-48f26480-8835-11e9-8ea7-fa13e4ac1881.png">

Luego se selecciona el recurso creado anteriormente se puede reconocer porque tiene el **nombre de la aplicación**,
tiene una descripción donde dice el servicio adquirido en este caso **Databases for MongoDB**, luego
de reconocer que es el correspondiente a la aplicación que se creó, da clic verificando que quede seleccionado y
luego clic en **Next**.

Luego de eso ya podrá ver que el recurso ya esta desplegado y activo en la aplicación.

<img width="600" alt="25" src="https://user-images.githubusercontent.com/50923637/59304676-573de780-8c5e-11e9-9a98-dfbf428bdac5.jpg">

`Nota: La credencial se crea automáticamente y la podrá ver en la siguiente imagen, se debe tener
en cuenta que al realizarlo fuera de la aplicación no se crean las credenciales de forma automática.`


<img width="600" alt="26" src="https://user-images.githubusercontent.com/50923637/59355521-bb0ef180-8cec-11e9-86c5-a8aa78b08c7d.jpg">

## Creación base de datos

Estando en el área de **App details** o **Detalles de la aplicación** deberá dar clic en el menú de despliegue del
recurso implementado, luego seleccionará la opción **Open dashboard**.

<img width="600" alt="27" src="https://user-images.githubusercontent.com/50923637/59357002-a5e79200-8cef-11e9-9bf2-7f06deb06633.jpg">

Estando en el dashboard de la aplicación se accede al area de **Connections** para buscar la conexión que desea activar o crear, por lo cual usted debe dar clic en **Create Connection** para que permita el funcionamiento correcto de su aplicación.

<img width="600" alt="29" src="https://user-images.githubusercontent.com/50923637/59366809-8147e600-8d00-11e9-8b03-065b9f5a1d68.jpg">

Luego se dirige al vinculo con el nombre de su aplicación y da clic en create para establecer la conexión con la base de datos para hacer efectivo el funcionamiento de la misma.

<img width="600" alt="30" src="https://user-images.githubusercontent.com/50923637/59367393-9a9d6200-8d01-11e9-90da-5311c91d85e4.jpg">

Luego se genera una ventana emergente en la cual ustes puede agregar algun archivo a la conexión para hacerla más compleja, pero en este caso no se realizara de esta manera, por lo cual usted dara clic en **Connect & restage app** para terminar el proceso de la conexión de la base de datos con su aplicación.

<img width="600" alt="31" src="https://user-images.githubusercontent.com/50923637/59367693-40e96780-8d02-11e9-9779-a73522b71a9a.jpg">

Luego debe acceder a lista de recursos y puede verificar si la aplicación esta correctamente aprovisionada con la base de datos que creo previamente.

<img width="600" alt="32" src="https://user-images.githubusercontent.com/50923637/59355085-feb52b80-8ceb-11e9-8dba-53dbe09fdf24.jpg">

Luego cuand oacceda a su aplicación podra ver en **Overview** en la sección de connections podrá ver que su conexión se establecio de manera correcta.

<img width="600" alt="33" src="https://user-images.githubusercontent.com/50923637/59368181-4a270400-8d03-11e9-91aa-7955eb570c74.jpg">

Luego debe acceder a la lista de recursos, se despliega el menú de apps, selecciona la aplicación creada, luego
de eso lo envía a la siguiente pantalla donde dará clic en la opción ver cadena de herramientas.

<img width="600" alt="39" src="https://user-images.githubusercontent.com/50923637/59038985-9244b300-8839-11e9-9c4f-d2f0fe7d8652.png">

En esta sección tendra diferentes herramientas para modificación de la aplicacion en este caso seleccionará la
opción **IDE web de eclipse Orion**, para modificar su aplicacion por medio de esta interfaz de código.

<img width="600" alt="40" src="https://user-images.githubusercontent.com/50923637/59038989-9375e000-8839-11e9-981c-7c54bf34f700.png">

Luego en la siguiente pantalla podra ver cada uno de los componentes de codigo que hacen funcionar la aplicación,
dentro de la sección se debe dirigir a la opción **client**.

<img width="600" alt="41" src="https://user-images.githubusercontent.com/50923637/59038992-94a70d00-8839-11e9-8b0f-56a571b9825b.png">

Luego se selecciona app.js, esta opción se selecciona para hacer el llamado a las APIS del servidor que harán
posible la comunicación con las bases de datos.

<img width="600" alt="42" src="https://user-images.githubusercontent.com/50923637/59039177-f36c8680-8839-11e9-9cf0-d41ff7a328a5.png">

En la sección donde se da el comentario **Add your code here**, agregará el siguiente código que lo encontrara
en la primera imagen, en la segunda imagen vera la sección resaltada para que pueda identificar en que parte
del código debe asignar el código anteriormente mencionado.

<img width="300" hight="700" alt="43a" src="https://user-images.githubusercontent.com/50923637/59039178-f5364a00-8839-11e9-9f7b-60f553c5fb31.png">

<img width="300" hight="700" alt="43b" src="https://user-images.githubusercontent.com/50923637/59039180-f8313a80-8839-11e9-9509-91bcec8e45a0.png">

<img width="600" alt="44" src="https://user-images.githubusercontent.com/50923637/59039181-f8c9d100-8839-11e9-9a1a-eee0fe911e0e.png">

Luego en la siguiente pantalla podra ver cada uno de los componentes de codigo que hacen funcionar la aplicación,
dentro de la sección se debe dirigir a la opción **server**.

<img width="600" alt="45" src="https://user-images.githubusercontent.com/50923637/59039538-a76e1180-883a-11e9-9de0-3a990d8ebb11.png">

Luego se selecciona server.js, esta opción se selecciona para provisionar las APIS que harán posible la comunicación
con las bases de datos.

`Nota: No olvide agregar la línea resaltada, esta línea permite la conexión, por medio de la
importación del módulo de la aplicación.`

<img width="600" alt="46" src="https://user-images.githubusercontent.com/50923637/59039551-ab9a2f00-883a-11e9-9407-715b0007586d.png">

En la sección donde se da el comentario **Add your code here**, agregará el siguiente código que lo encontrara
en la primera imagen, en la segunda imagen vera la sección resaltada para que pueda identificar en que parte
del código debe asignar el código anteriormente mencionado.

<img width="600" alt="47" src="https://user-images.githubusercontent.com/50923637/59039545-a9d06b80-883a-11e9-858b-472c35f71662.png">

<img width="600" alt="48" src="https://user-images.githubusercontent.com/50923637/59039549-ab019880-883a-11e9-9b52-d2f1801d5eaa.png">

Luego en server se deber ir a la sección Model, luego se selecciona Coments.js se da clic derecho, se selecciona
la opción renombrar y cambiarlo al nombre de la aplicación.js.

<img width="600" alt="49" src="https://user-images.githubusercontent.com/50923637/59039738-ff0c7d00-883a-11e9-9e98-06e675d8b68c.png">

Dentro de la sección que anteriormente era llamada coments.js se debe agregar el siguiente código, el cual es la
estructura del esquema que define la base de datos de la aplicación.

<img width="450" alt="50" src="https://user-images.githubusercontent.com/50923637/59039740-ffa51380-883a-11e9-93f9-477b448032f0.png">

Luego se debe dirigir a la carpeta routes donde seleccionara el archivo mongo js para modificarlo.

<img width="600" alt="51" src="https://user-images.githubusercontent.com/50923637/59039746-016ed700-883b-11e9-92d4-938eb16cee2f.png">

Las modificaciones que debe hacer son las siguientes, estas modificaciones le permitirá establecer la conexión
con el modelo de la base de datos.

* LINEA 26: Se cambia la constante coments por la por var Nombre de la aplicación = require(’./model/Nombre
de la aplicación’) ;
* LINEA 32: Se cambia comments por el nombre de la aplicación.
* LINEA 42: Se cambia el estado de ssl, que está en false, se cambia por true.

Luego se cambia el archivo component.html el cual es la interfaz gráfica donde se crea el formulario que ingresa
los datos de la aplicación.

<img width="600" alt="52" src="https://user-images.githubusercontent.com/50923637/59039750-03d13100-883b-11e9-9815-a8e86a50d758.png">

Lo que está dentro del component.html se modifico con el siguiente código, el cual fue el código realizado para
la aplicación que se empleó como ejemplo para la realización de esta guía de usuario.

<img width="450" alt="53" src="https://user-images.githubusercontent.com/50923637/59039954-61657d80-883b-11e9-96e0-4322da9d33fc.png">

<img width="450" alt="54" src="https://user-images.githubusercontent.com/50923637/59039955-61fe1400-883b-11e9-8c01-5db59fd417f6.png">

Finalmente podrá ver la aplicación de ejemplo que se desplego, esta aplicación es para hacer una base de datos
de películas en una página Web con la ayuda de las herramientas que proporciona IBM Cloud.

<img width="600" alt="55" src="https://user-images.githubusercontent.com/50923637/59039957-632f4100-883b-11e9-9f55-badea6134873.png">

## Codigos modificación Mean App

---

### client/Component.html

```
<section>
    <header id="flex-header">
        <div class="cloud-header"></div>
        <h2>IBM Cloud - App MEAN</h2>
    </header>
    <main>
		 <div ng-init="get()" style="display: flex;justify-content: center;">
		 	<div style="width: 800px;">
		    	<table>
				<tr>
		    		  <td  cols="12" align="right">
		    		  <label>Id</label>
		    		  </td>
		    		  <td>
		              <input ng-model="id" type="text" name="id" cols="40">
		          	  </td>
		        </tr>
		    	<tr>
		    		  <td  cols="12" align="right">
		    		  <label>Title</label>
		    		  </td>
		    		  <td>
		              <input ng-model="title" type="text" name="title" cols="40">
		          	  </td>
		        </tr>
		        <tr>
		        	  <td  cols="12" align="right">
		        	  <label>Description</label>
		        	  </td>
		        	  <td>
		              <textarea ng-model="description"  name="description" cols="80"></textarea>
		          	  </td>
		         </tr>
 				 <tr>
		        	  <td  cols="12" align="right">
		    		  <label>Director</label>
		    		  </td>
		    		  <td>		    	
		              <input ng-model="director" type="text" name="director" cols="30">
		              </td>
		         </tr>
 				 <tr>
		        	  <td  cols="12" align="right">
		    		  <label>Year</label>		        
		    		  </td>
		    		  <td>
		              <input ng-model="year" type="text" name="year" cols="6">
		          	  </td>
		         </tr>
		         <tr>
		         	<td></td>
		         	<td>
			        <button ng_click="get()" style="font-size: 14px;background-color: #e7e7e7; color: black;border: 2px solid black;">
			        	List
			        </button>
		
			        <button ng_click="add()" style="font-size: 14px;background-color: #e7e7e7; color: black;border: 2px solid black;">
			        	Add
			        </button>	        

			        <button ng_click="update()" style="font-size: 14px;background-color: #e7e7e7; color: black;border: 2px solid black;">
			        	Update
			        </button>	
			      	<button ng_click="delete()" style="font-size: 14px;background-color: #e7e7e7; color: black;border: 2px solid black;">
			        	Delete
			        </button>	
			        </td>         
		         </tr>
		         </table>	        
		        <table style="border:1px solid black;">
		        <tr>
						<th>id</th>
						<th cols="30">title </th>
						<th cols="50">description</th>
						<th cols="25">director<th>
						<th cols="6">year</th>		        
				</tr>
		        <tr ng-repeat="movie in movies">
						<td>{{movie._id}}</td>
						<td>{{movie.title}}</td>
						<td>{{movie.description}}</td>
						<td>{{movie.director}}</td>
						<td>{{movie.year}}</td>
		        </tr>
		        </table>
		    </div>
		 </div>
	</main>		 
</section>

```

### client/App.js

```

 */
 ľ Copyright IBM Corp . 2018
 Licensed under the Apache License , Version 2.0 (the " License ");
 you may not use this file except in compliance with the License .
 You may obtain a copy of the License at
 http :// www . apache .org / licenses / LICENSE -2.0
 Unless required by applicable law or agreed to in writing , software
 distributed under the License is distributed on an "AS IS" BASIS ,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND , either express or implied .
 See the License for the specific language governing permissions and
 limitations under the License .
 */

 require (’./ default .css ’);

 angular . module (’App ’, [’ui. router ’, ’MainView ’])
 . config ( function ( $stateProvider , $urlRouterProvider ) {
 ’ngInject ’;
 $stateProvider . state (’MainState ’, {
 url : ’’,
 templateUrl : ’/ templates / component . html ’,
 controller : ’MainCtrl ’
 });
 $urlRouterProvider . otherwise (’/’);
 });

 angular . module (’MainView ’, [])
 . controller (’MainCtrl ’, [’$scope ’, ’$http ’, function ($scope , $http ) {

 $scope .id = "" ;
 $scope . title = "" ;
 $scope . director = "" ;
 $scope . description = "" ;
 $scope . year = "" ;

 $scope . data = "" ;

 $scope .add = function () {

 $http ({
 method : ’POST ’,
 url : ’/api / movies /’,
 data : {
 ’title ’: $scope .title ,
 ’director ’: $scope . director ,
 ’description ’: $scope . description ,
 ’year ’: $scope . year
 }
 })
 . then ( function ( response ) {
 $scope .get () ;

 }, function ( error ) {
 console . error (’get movies failed : %s’, error . message ) ;
 }) ;

 } ;

 $scope .get = function () {

 $http ({
 method : ’GET ’,
 url : ’/api / movies /’

 })
 . then ( function ( response ){

 $scope . movies = response . data ;
 $scope . data = $scope . movies [0]. title ;

 console . info (’get movies sussess : %s’, $scope . movies [0]. title ) ;

 }, function ( error ) {

 $scope . data = error . message ;
 console . info (’get movies failed : %s’, error . message ) ;
 }) ;
 } ;


 $scope . update = function () {

 $http ({
 method : ’PUT ’,
 url : ’/api / movies /’ + $scope .id ,
 data : {
 ’_id ’: $scope .id ,
 ’title ’: $scope .title ,
 ’director ’: $scope . director ,
 ’description ’: $scope . description ,
 ’year ’: $scope . year
 }
 })
 . then ( function ( response ) {
 $scope .get () ;

 }, function ( error ) {
 console . error (’update movies failed : %s’, error . message ) ;
 }) ;
 } ;



 $scope . delete = function () {

 $http ({
 method : ’DELETE ’,
 url : ’/api / movies /’+ $scope .id ,
 data : {
 ’_id ’: $scope .id ,
 }
 })
 . then ( function ( response ) {
 $scope .get () ;

 }, function ( error ) {
 console . error (’delete movies failed : %s’, error . message ) ;
 }) ;
 } ;
 }]) ;

```

### server/model/movies.js

```

/*
  Licensed to the Apache Software Foundation (ASF) under one
  or more contributor license agreements.  See the NOTICE file
  distributed with this work for additional information
  regarding copyright ownership.  The ASF licenses this file
  to you under the Apache License, Version 2.0 (the
  "License"); you may not use this file except in compliance
  with the License.  You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

  Unless required by applicable law or agreed to in writing,
  software distributed under the License is distributed on an
  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
  KIND, either express or implied.  See the License for the
  specific language governing permissions and limitations
  under the License.
 */

//model/comments.js

'use strict';

var mongoose = require('mongoose');
var Schema = mongoose.Schema;

var MoviesSchema = new Schema({
  title: String,
  description: String,
  director: String,
  year: String
});

var model = mongoose.model('Movie', MoviesSchema);
module.exports = model ;

```

### server/server.js

```

 // Uncomment following to enable zipkin tracing , tailor to fit your network configuration :
 // var appzip = require (’ appmetrics - zipkin ’)({
 // host : ’localhost ’,
 // port : 9411 ,
 // serviceName :’ frontend ’
 // });

 require (’appmetrics - dash ’). attach ();
 require (’appmetrics - prometheus ’). attach ();
 const appName = require (’./../ package ’). name ;
 const http = require (’http ’);
 const express = require (’express ’);
 const log4js = require (’log4js ’);
 const localConfig = require (’./ config / local . json ’);
 const path = require (’path ’);

 // inicio
 // Importar Modulo Movies
 var Movie = require (’./ model / movies ’) ;


 const logger = log4js . getLogger ( appName );
 logger . level = process .env . LOG_LEVEL || ’info ’
 const app = express ();
 const server = http . createServer (app );

 app .use ( log4js . connectLogger (logger , { level : logger . level }));
 const serviceManager = require (’./ services / service - manager ’);
 require (’./ services / index ’)( app );
 require (’./ routers / index ’)(app , server );

 // Movies APIs

 app .get ("/api / movies ", function (req , res , next ) {

 Movie . find ( function (err , post ) {
 if (err ) return next (err );
 res . json ( post );
 });

 });


 app .get ("/api / movies /: id", function (req , res , next ) {

 Movie . findById (req . params .id , function (err , post ) {
 if (err ) return next (err );
 res . json ( post );
 });

 });

 app . post ("/api / movies ", function (req , res , next ) {

 Movie . create (req .body , function (err , post ) {

 if (err ) return next (err );
 res . json ( post );
 });

 });

 // update Movie
 app .put ("/api / movies /: id", function (req , res , next ) {
 Movie . findByIdAndUpdate (req . params .id , req .body , function (err , post ) {
 if (err ) return next (err );
 res . json ( post );
 });
 });

 // DELETE Movie

 app . delete ("/api / movies /: id", function (req , res , next ) {
 Movie . findByIdAndRemove (req . params .id , function (err , post ) {
 if (err ) return next (err );
 res . json ( post );
 });
 });

 // final

 const port = process .env . PORT || localConfig . port ;
 server . listen (port , function (){
 logger . info (‘ DEMOPELICULAS listening on http :// localhost :${ port }/ appmetrics -dash ‘);
 logger . info (‘ DEMOPELICULAS listening on http :// localhost :${ port }‘);
 });

 app .use ( function (req , res , next ) {
 res . sendFile ( path . join ( __dirname , ’../ public ’, ’404. html ’));
 });

 app .use ( function (err , req , res , next ) {
 res . sendFile ( path . join ( __dirname , ’../ public ’, ’500. html ’));
 });

 module . exports = server ;
```

