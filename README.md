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
