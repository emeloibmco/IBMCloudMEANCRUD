# IBMCloudMEANCRUD
Hands On para construir aplicación utilizando el Stack MEAN en IBM Cloud

## Índice

* Creación y despliegue de la MEAN Stack App.
* Creación base de datos y enlace con el MEAN Stack App.

## 1. Introducción
En la siguiente guía puede observar cómo se realiza la creación, el despliegue y la modificación de un Mean
stack, con mongo Db, Express.js, Angular y node.js en IBM Cloud.

## 2. Creación y despliegue MEAN Stack App

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

Luego en la ventana aparece el recurso que desea agregar, deberá buscar la opción **Compose for Mongo Db**,
seleccionará esta opción y da clic en **Next** o **Siguiente**.

<img width="600" alt="21" src="https://user-images.githubusercontent.com/50923637/59036120-50653e00-8834-11e9-9baa-786bf6d59af8.png">

Después de eso se realiza el despliegue, en la ventana las opciones deben seleccionar la región, está ya seleccionado
el resource group o grupo de recursos anteriormente asignado luego de eso deberá dar clic en la opción **Create**
o **Crear**.


`Nota: Para poder agregar un recurso a una aplicación se debe tener en cuenta que la cuenta
debe contar con permisos o debe ser una cuenta paga es decir con recursos para poder realizar
esta acción de provisionar recursos.`

<img width="600" alt="22" src="https://user-images.githubusercontent.com/50923637/59036615-47c13780-8835-11e9-84b3-c930f03d61c7.png">

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
tiene una descripción donde dice el servicio adquirido en este caso **Compose for MongoDB**, luego
de reconocer que es el correspondiente a la aplicación que se creó, da clic verificando que quede seleccionado y
luego clic en **Next**.

<img width="600" alt="24" src="https://user-images.githubusercontent.com/50923637/59036624-4a239180-8835-11e9-9c6f-926a0927ff95.png">

Luego de eso ya podrá ver que el recurso ya esta desplegado y activo en la aplicación.

<img width="600" alt="25" src="https://user-images.githubusercontent.com/50923637/59036628-4bed5500-8835-11e9-80da-031d37931fc8.png">

`Nota: La credencial se crea automáticamente y la podrá ver en la siguiente imagen, se debe tener
en cuenta que al realizarlo fuera de la aplicación no se crean las credenciales de forma automática.`


<img width="600" alt="26" src="https://user-images.githubusercontent.com/50923637/59036927-d766e600-8835-11e9-9420-26d22071002a.png">

## Creación base de datos

Estando en el área de **App details** o **Detalles de la aplicación** deberá dar clic en el menú de despliegue del
recurso implementado, luego seleccionará la opción **Open dashboard**.

<img width="600" alt="27" src="https://user-images.githubusercontent.com/50923637/59038349-886e8000-8838-11e9-87f5-954f0a028c8c.png">

Luego de esto se abre una ventana emergente la cual lo ubicará por defecto en la opción **Manage** o **Gestionar**
en la cual usted podrá verificar que el estado de los tasks este completado.

<img width="600" alt="28" src="https://user-images.githubusercontent.com/50923637/59036935-d9c94000-8835-11e9-84b8-b858f32108e2.png">

Estando en la sección de **Manage** o **Gestionar**,se debe buscar la dirección HTTP de la aplicación que fue
creada, para tener los datos de password, usuario, dirección de la base de datos para establecer la comunicación
de la aplicación de Node.js y la base de datos.

En la siguiente imagen podrá ver en el campo de color azul va el nombre usuario asignado,en color amarillo el
Password o contraseña de usuario asignado y finalmente vera en color verde la dirección IP correspondiente a
la base de datos.

<img width="600" alt="29" src="https://user-images.githubusercontent.com/50923637/59036940-dafa6d00-8835-11e9-972f-d91a376f0e85.png">

Luego se debe dirigir a la **lista de recursos** o **resource list** para poder acceder a la aplicación que creo, esto
por medio del despliegue del **menú de hamburguesa**.

<img width="600" alt="30" src="https://user-images.githubusercontent.com/50923637/59038475-b5229780-8838-11e9-92ed-e29c68cf14b6.png">

Ya estando en la lista de recursos seleccione su aplicación y de clic en ella para poder acceder a la información
de su aplicación.

<img width="600" alt="31" src="https://user-images.githubusercontent.com/50923637/59038480-b6ec5b00-8838-11e9-83c3-70d8d6a57731.png">

Luego estando en su aplicación selecciona tiempos de ejecución y en tiempos de ejecución selecciona la opción
variable de entorno.

<img width="600" alt="32" src="https://user-images.githubusercontent.com/50923637/59038481-b81d8800-8838-11e9-9929-4d21bbcb9ece.png">

Luego se debe dar clic en **variables de entorno** donde verá la siguiente pagina de opciones, en la cual luego
se debe dar clic en **añadir** en los espacios que se generan debe agregar,**MongoDB URL, MongoDB user y
MongoDB password**.

`Nota: Para encontrar el MongoDB URL, password y user podrá ubicarlos en la sección de
HTTP anteriormente mencionada donde están indicados con colores cual corresponde a la opción
deseada.`

<img width="600" alt="33" src="https://user-images.githubusercontent.com/50923637/59038486-b94eb500-8838-11e9-8b80-23daf8150e30.png">

En la siguiente imagen podrá ver la forma en que se agregan las opciones que se estaban mencionando anteriormente.

**Nota: se debe tener en cuenta que en el espacio en purpura, por defecto la base de datos lo
asigna como ADMIN.**

<img width="600" alt="34" src="https://user-images.githubusercontent.com/50923637/59038810-41cd5580-8839-11e9-8943-4405166ca5ce.png">

Luego se debe dar clic en la opción de conexiones ubicado en la parte izquierda de la pantalla.

<img width="600" alt="35" src="https://user-images.githubusercontent.com/50923637/59038811-4265ec00-8839-11e9-9693-bc6255696e1f.png">

Luego se debe dar clic en crear conexión, luego se desplegaran las aplicaciones compatibles con la anteriormente
creada.

<img width="600" alt="36" src="https://user-images.githubusercontent.com/50923637/59038823-42fe8280-8839-11e9-880d-21711f59b60d.png">

Luego dentro de los servicios compatibles seleccionará el servicio para la aplicación que previamente se creó, se
da clic en el para seleccionarlo y después de tenerlo seleccionado se da clic en crear.

<img width="600" alt="37" src="https://user-images.githubusercontent.com/50923637/59038826-442faf80-8839-11e9-866e-c9c722e7cf0c.png">

Luego se da clic en la opción volver a transferir, esta opción lo que realiza es el reinicio de la aplicación y los
servicios para establecer una conexión de todos ellos.

`Nota: debe esperar unos segundos mientras se realiza el proceso e reinicio que se habilito al dar
clic en volver a transferir.`

<img width="600" alt="38" src="https://user-images.githubusercontent.com/50923637/59038981-907aef80-8839-11e9-9b51-e973f4e64d73.png">

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

### Mongo.js

```
1
2 */
3 Licensed to the Apache Software Foundation (ASF ) under one
4 or more contributor license agreements . See the NOTICE file
5 distributed with this work for additional information
6 regarding copyright ownership . The ASF licenses this file
7 to you under the Apache License , Version 2.0 (the
8 " License "); you may not use this file except in compliance
9 with the License . You may obtain a copy of the License at
10 http :// www . apache .org / licenses / LICENSE -2.0
11 Unless required by applicable law or agreed to in writing ,
12 software distributed under the License is distributed on an
13 "AS IS" BASIS , WITHOUT WARRANTIES OR CONDITIONS OF ANY
14 KIND , either express or implied . See the License for the
15 specific language governing permissions and limitations
16 under the License .
17 */
18
19 ’use strict ’;
20
21 const mongoose = require (’mongoose ’);
22 const bodyParser = require (’body - parser ’);
23 const session = require (’express - session ’);
24 const MongoStore = require (’connect - mongo ’)( session );
25
26 // Sample Model
27 const Comment = require (’../ model / movies ’);
28
29 // user set constiables
30 const mongoURL = process .env . MONGO_URL || ’localhost ’;
31 const mongoUser = process .env . MONGO_USER || ’’;
32 const mongoPass = process .env . MONGO_PASS || ’’;
33 const mongoDBName = process .env . MONGO_DB_NAME || ’comments ’;
34
35 module . exports = function (app ){
36 // set up other middleware
37 app .use ( bodyParser . urlencoded ({ extended : true }));
38 app .use ( bodyParser . json ());
39
40 const options = {
41 useMongoClient : true ,
42 ssl : true ,
43 sslValidate : false ,
44 poolSize : 1,
45 reconnectTries : 1
46 };
47
48 // connect to the MongoDB
49 let mongoConnect = ’mongodb :// localhost :27017 ’;
50 if ( mongoURL !== ’’ && mongoUser !== ’’ && mongoPass != ’’) {
51 mongoConnect = ‘mongodb ://${ mongoUser }:${ mongoPass }${ mongoURL }/${ mongoDBName }‘;
52 } else if ( mongoURL !== ’’) {
53 mongoConnect = ‘mongodb ://${ mongoURL }/${ mongoDBName }‘;
54 }
55
56 mongoose . Promise = global . Promise ;
57 mongoose . connect ( mongoConnect , options )
58 . catch (( err ) => {
59 if (err ) console . error (err );
60 });
61
62 var db = mongoose . connection ;
63 db.on(’error ’, ( error ) => {
64 console . error ( error );
65 });
66
67 var sess = {
68 store : new MongoStore ({ mongooseConnection : mongoose . connection }) ,
69 name : ’mean example ’,
70 secret : ’ninpocho ’,
71 resave : false ,
72 saveUnitialized : true ,
31
73 cookie : {}
74 };
75
76 app .use ( session ( sess ));
77
78 console . info (’Connection established with mongodb ’);
79 console . info (‘ Connection details : ${ mongoConnect }‘);
80
81 };

```

### App.js

```
1
2 */
3 ľ Copyright IBM Corp . 2018
4 Licensed under the Apache License , Version 2.0 (the " License ");
5 you may not use this file except in compliance with the License .
6 You may obtain a copy of the License at
7 http :// www . apache .org / licenses / LICENSE -2.0
8 Unless required by applicable law or agreed to in writing , software
9 distributed under the License is distributed on an "AS IS" BASIS ,
10 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND , either express or implied .
11 See the License for the specific language governing permissions and
12 limitations under the License .
13 */
14
15 require (’./ default .css ’);
16
17 angular . module (’App ’, [’ui. router ’, ’MainView ’])
18 . config ( function ( $stateProvider , $urlRouterProvider ) {
19 ’ngInject ’;
20 $stateProvider . state (’MainState ’, {
21 url : ’’,
22 templateUrl : ’/ templates / component . html ’,
23 controller : ’MainCtrl ’
24 });
25 $urlRouterProvider . otherwise (’/’);
26 });
27
28 angular . module (’MainView ’, [])
29 . controller (’MainCtrl ’, [’$scope ’, ’$http ’, function ($scope , $http ) {
30
31 $scope .id = "" ;
32 $scope . title = "" ;
33 $scope . director = "" ;
34 $scope . description = "" ;
35 $scope . year = "" ;
36
37 $scope . data = "" ;
38
39 $scope .add = function () {
40
41 $http ({
42 method : ’POST ’,
43 url : ’/api / movies /’,
44 data : {
45 ’title ’: $scope .title ,
46 ’director ’: $scope . director ,
47 ’description ’: $scope . description ,
48 ’year ’: $scope . year
49 }
50 })
51 . then ( function ( response ) {
52 $scope .get () ;
53
54 }, function ( error ) {
55 console . error (’get movies failed : %s’, error . message ) ;
56 }) ;
57
58 } ;
59
60 $scope .get = function () {
61
62 $http ({
63 method : ’GET ’,
64 url : ’/api / movies /’
32
65 })
66 . then ( function ( response ){
67
68 $scope . movies = response . data ;
69 $scope . data = $scope . movies [0]. title ;
70
71 console . info (’get movies sussess : %s’, $scope . movies [0]. title ) ;
72
73 }, function ( error ) {
74
75 $scope . data = error . message ;
76 console . info (’get movies failed : %s’, error . message ) ;
77 }) ;
78 } ;
79
80
81 $scope . update = function () {
82
83 $http ({
84 method : ’PUT ’,
85 url : ’/api / movies /’ + $scope .id ,
86 data : {
87 ’_id ’: $scope .id ,
88 ’title ’: $scope .title ,
89 ’director ’: $scope . director ,
90 ’description ’: $scope . description ,
91 ’year ’: $scope . year
92 }
93 })
94 . then ( function ( response ) {
95 $scope .get () ;
96
97 }, function ( error ) {
98 console . error (’update movies failed : %s’, error . message ) ;
99 }) ;
100 } ;
101
102
103
104 $scope . delete = function () {
105
106 $http ({
107 method : ’DELETE ’,
108 url : ’/api / movies /’+ $scope .id ,
109 data : {
110 ’_id ’: $scope .id ,
111 }
112 })
113 . then ( function ( response ) {
114 $scope .get () ;
115
116 }, function ( error ) {
117 console . error (’delete movies failed : %s’, error . message ) ;
118 }) ;
119 } ;
120 }]) ;

```

### Movies.js

```

1
2 /*
3 Licensed to the Apache Software Foundation (ASF ) under one
4 or more contributor license agreements . See the NOTICE file
5 distributed with this work for additional information
6 regarding copyright ownership . The ASF licenses this file
7 to you under the Apache License , Version 2.0 (the
8 " License "); you may not use this file except in compliance
9 with the License . You may obtain a copy of the License at
10
11 http :// www . apache .org / licenses / LICENSE -2.0
12
13 Unless required by applicable law or agreed to in writing ,
14 software distributed under the License is distributed on an
15 "AS IS" BASIS , WITHOUT WARRANTIES OR CONDITIONS OF ANY
16 KIND , either express or implied . See the License for the
17 specific language governing permissions and limitations
33
18 under the License .
19 */
20
21 ’use strict ’;
22
23 var mongoose = require (’mongoose ’);
24 var Schema = mongoose . Schema ;
25
26 var MoviesSchema = new Schema ({
27 title : String ,
28 description : String ,
29 director : String ,
30 year : String
31 });
32
33 var model = mongoose . model (’Movie ’, MoviesSchema );
34 module . exports = model ;

```

### Server.js

```
1
2 // Uncomment following to enable zipkin tracing , tailor to fit your network configuration :
3 // var appzip = require (’ appmetrics - zipkin ’)({
4 // host : ’localhost ’,
5 // port : 9411 ,
6 // serviceName :’ frontend ’
7 // });
89
require (’appmetrics - dash ’). attach ();
10 require (’appmetrics - prometheus ’). attach ();
11 const appName = require (’./../ package ’). name ;
12 const http = require (’http ’);
13 const express = require (’express ’);
14 const log4js = require (’log4js ’);
15 const localConfig = require (’./ config / local . json ’);
16 const path = require (’path ’);
17
18 // inicio
19 // Importar Modulo Movies
20 var Movie = require (’./ model / movies ’) ;
21
22
23 const logger = log4js . getLogger ( appName );
24 logger . level = process .env . LOG_LEVEL || ’info ’
25 const app = express ();
26 const server = http . createServer (app );
27
28 app .use ( log4js . connectLogger (logger , { level : logger . level }));
29 const serviceManager = require (’./ services / service - manager ’);
30 require (’./ services / index ’)( app );
31 require (’./ routers / index ’)(app , server );
32
33 // Movies APIs
34
35 app .get ("/api / movies ", function (req , res , next ) {
36
37 Movie . find ( function (err , post ) {
38 if (err ) return next (err );
39 res . json ( post );
40 });
41
42 });
43
44
45 app .get ("/api / movies /: id", function (req , res , next ) {
46
47 Movie . findById (req . params .id , function (err , post ) {
48 if (err ) return next (err );
49 res . json ( post );
50 });
51
52 });
53
54 app . post ("/api / movies ", function (req , res , next ) {
55
56 Movie . create (req .body , function (err , post ) {
34
57 if (err ) return next (err );
58 res . json ( post );
59 });
60
61 });
62
63 // update Movie
64 app .put ("/api / movies /: id", function (req , res , next ) {
65 Movie . findByIdAndUpdate (req . params .id , req .body , function (err , post ) {
66 if (err ) return next (err );
67 res . json ( post );
68 });
69 });
70
71 // DELETE Movie
72
73 app . delete ("/api / movies /: id", function (req , res , next ) {
74 Movie . findByIdAndRemove (req . params .id , function (err , post ) {
75 if (err ) return next (err );
76 res . json ( post );
77 });
78 });
79
80 // final
81
82 const port = process .env . PORT || localConfig . port ;
83 server . listen (port , function (){
84 logger . info (‘ DEMOPELICULAS listening on http :// localhost :${ port }/ appmetrics -dash ‘);
85 logger . info (‘ DEMOPELICULAS listening on http :// localhost :${ port }‘);
86 });
87
88 app .use ( function (req , res , next ) {
89 res . sendFile ( path . join ( __dirname , ’../ public ’, ’404. html ’));
90 });
91
92 app .use ( function (err , req , res , next ) {
93 res . sendFile ( path . join ( __dirname , ’../ public ’, ’500. html ’));
94 });
95
96 module . exports = server ;
```
