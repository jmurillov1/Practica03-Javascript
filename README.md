# Practica03-Javascript

 	FORMATO DE INFORME DE PRÁCTICA DE LABORATORIO / TALLERES / CENTROS DE SIMULACIÓN – PARA ESTUDIANTES

CARRERA:  INGENIERÍA DE SISTEMAS
	ASIGNATURA:  HYPERMEDIAL 

NRO. PRÁCTICA:	2	TÍTULO PRÁCTICA:  Resolución de problemas sobre CSS3

OBJETIVO ALCANZADO:
Entender y organizar de una mejor manera los sitios de web en Internet 
Diseñar adecuadamente elementos gráficos en sitios web en Internet.
Crear sitios web aplicando estándares actuales.

ACTIVIDADES DESARROLLADAS
1. Crear un repositorio en GitHub con el nombre “Practica03 – Javascript”
Para realizar este paso previamente creamos una cuenta en GitHub, ahora conectado a la cuenta en línea procedemos a crear el repositorio donde guardaremos la práctica.
 
Luego tendremos la siguiente pantalla:







 
Con esto ya hemos creado nuestro repositorio. En este lugar nos dará la url del repositorio que es necesaria para configurar la forma de subir los archivos.
2. Crear una carpeta para la solución de cada ejercicio antes mencionado.
 
Evidencia de la creación de las carpetas para cada ejercicio.
3. Realizar un commit y push por cada requerimiento de los puntos antes descritos. 
Para el desarrollo de esta práctica tendremos 3 puntos ejercicios a realizar haciendo uso de Javascript.
Para esto debemos abrir el cmd y colocar los siguientes comandos, en el caso de Windows:
-	git init
-	git add .
-	git commit -m "Nombre-Proyecto"
-	git remote add origin “url del respositorio”
-	git push -u origin master
Estos para la primera vez que se vaya a trabajar con el proyecto, después solo es necesario correr:
-	git add .
-	git commit -m "Nombre-Proyecto"
-	git push -u origin master
Y para que esto funcione previamente debes haber instalado y configurado “Git for Windows”.
Ahora luego de correr los comandos tendremos:
 
Con el init iniciamos el repositorio vacío.
Con el add los añadimos.
Con el commit creamos los datos dentro del repositorio.
Con el remote le damos la dirección de donde subir los archivos.
Y con el push guardamos los datos en el repositorio.
Si todo corre bien deberíamos obtener lo siguiente:
 
Como pueden darse cuenta la pagina web en GitHub se actualiza con los nuevos datos subidos, con esto hemos cargado en la pagina el primer punto de la práctica.
El proyecto se fue haciendo poco a poco, como vimos primero voy a explicar el primer ejercicio que es la calculadora:
1.	Calculadora
Se pide construir una calculadora en el lenguaje de programación de JavaScript con base a un formulario HTML usando botones y una caja de texto. Además, para   que   permita realizar   operaciones   aritméticas de complejidad básica, como: suma, resta, multiplicación, división, raíz cuadrada, entre otros. A continuación, se muestra un ejemplo de las operaciones que debe realizar la calculadora.
Parte HTML5:
  
El archivo se llama index.html, para esta parte hicimos uso de las etiquetas antes vistas y ordenamos los distintos componentes que conformar la calculadora, basada en la calculadora estándar de Windows 7. Escribimos las etiquetas básicas de estructura de un archivo html, y en la etiqueta body en dos se configura todo. Aquí dentro se colocó todo en una etiqueta div para un manejo más fácil. Luego, en un form se coloco todo lo requerido por la calculadora, en el orden para que quede en base a la calculadora de referencia antes especificada. En una etiqueta h6 puse el titulo como el icono de la calculadora, y luego en etiquetas p puse las diferentes líneas de componentes que conforman la calculadora. Dentro de los p para hacer las teclas se hizo uso de etqiuetas input de tipo button y para la pantalla de impresión también una etiqueta p con un gran espacio, para que muestre los resultados que se calculen.
En la etiqueta head colocamos la importación del archivo .css y el archivo .js los cuales se encargaran de que funcione correctamente la calculadora.
Además en la parte de los input se llama a los métodos de nuestro archivo .js, todos los eventos son onclick, ejemplo de uso: onclick=”porcent()”.

CSS3
  
 
 
Para el archivo CSS tenemos los estilos que llevara para que la calculadora que con una buena estética y tenga parecido a la calculadora de referencia.
Para mayor facilidad de manejo se hizo uso de los selectores antes vistos, con lo cual se fue dando forma al requerimiento solicitado. Hicimos uso de colores para dar el color parecido a la calculadora de referencia.
Para la ubicación del botón igual se hizo uso de el posicionamiento relativo, y para ordenar según filas los botones si hizo uso de la propiedad de pantalla flex.
Con la ayuda de pseudo-clases se dio el efecto de cambio de color de los botones al colocar el mouse sobre el botón, la pseudo-clase usada es hover.












JAVASCRIPT
 
Para esto use ayuda de internet, aquí tenemos 2 funciones la primera se encarga de obtener el valor de la pantalla de resultados. Luego se declaran las variables necesarias para trabajar y la segunda función se encarga mostrar los datos según el botón que se de click y lo que sea posible según la calculadora.
  
Continuamos con las funciones, ahora tenemos la función operar() que se le pasa el tipo de operación a realizar, luego la función igualar() que se encarga de revisar si existen operaciones pendientes y las evalúa. Seguido tenemos la función raíz que se encarga de calcular la raíz cuadrada del valor en pantalla.
 
Continuando, tenemos la función porcent() que saca el porcentaje(división para 100 del número en pantalla) según el valor en pantalla, la función opuest() que saca el opuesto del valor en pantalla, seguido la función inve() que saca la división de 1 para el numero en pantalla, luego la función retro() que borra el ultimo digito escrito. 
 
Por último, la función borradoParcial() que borra la pantalla y finalmente la función borradoTotal() que devuelve la pantalla a 0.

Commit y Push
 
 
Ahí hemos subido el primer ejercicio a nuestro GitHub.
2.	Validaciones
Diseñar una interfaz en HTML que permita ingresar los siguientes campos en un formulario: cedula, nombres, apellidos, dirección, teléfono, fecha de nacimiento y correo electrónico.  Luego, usando funciones de JavaScript se debe validar que todos los campos han sido ingresados, además; que los 
valores ingresados en cada campo del formulario sean correctos teniendo en 
cuenta las siguientes condiciones:
a.	Se debe validar qué, en el campo de la cedula, se ingrese sólo número y que la misma sea correcta, en base, al último dígito verificador.
b.	Se debe validar qué, en el campo de nombres, ingrese únicamente dos nombres y que permita ingresar sólo letras.
c.	Se debe validar qué, en el campo de apellido, ingrese únicamente dos apellidos y que permita ingresar sólo letras.
d.	Se debe validar qué, en el campo del teléfono, permita ingresar sólo números.
e.	Se debe validar que la fecha de nacimiento ingrese en el formato dd/mm/yyyy.
f.	Se debe validar qué, en el campo correo electrónico, permita ingresar un correo válido. Se considera un correo válido, cuando comienza por tres o más valores alfanuméricos, luego un @, seguido por  la  extensión “ups.edu.ec” o “est.ups.edu.ec”.
Indicaciones:
• Para realizar las validaciones de solo letras, o sólo números. Se las debe realizar en tiempo real, es decir, a medida que el usuario escribe en el campo.
• Todos los campos de entrada dentro del formulario deben de ser de tipo “text”.
• Las demás validaciones se realizarán al momento de “enviar” (submit) la información del formulario hacia una página php. Si no cumple las validaciones, se mostrará un mensaje debajo de cada campo con el error y se pintará el campo con un borde rojo que representará que el campo tiene un error. Si se cumple las validaciones, se enviará a una página php, en donde se mostrará únicamente un mensaje que diga “Bienvenido, ¡pasaste las validaciones!”.



HTML5
 
 
Creamos el archivo .html necesario llamado crear_usuario.html del cual realizaremos las validaciones y nos devolverá un mensaje si está bien al hacer el envió de datos a través del formulario. 
En la etiqueta body importamos el archivo .css y .js para el funcionamiento del trabajo. Para nuestro caso utilizaremos una etiqueta form con el método POST para enviar los datos, en acción la ruta del archivo donde se enviar los datos con extensión .php, y el evento a usar que es onsubmit=”validarCamposObligatorios()” para la mayoría de datos a enviar, solo para los nombres apellidos y números se usara el envento onkeyup porque se debe validar en tiempo real. Utilizamos un label para poner a que se refieren los campos de entrada de datos, en inputs los campos para ingreso de datos, de tipo text, al final un dos input, uno de tipo submit para enviar y uno de tipo reset para cancelar.

CSS3
 
El archivo .css para este ejercicio es muy básico ya que los estilos según las validaciones las vamos a dar con ayuda de javascript. En este archivo le damos el estilo a nuestro formulario.









PHP
 
Este archivo en donde se llegará, si al pasar el formulario por las validaciones todo resulta bien. Nos devuelve un saludo de que todo fue un éxito. 

JAVASCRIPT
 
 
Esta es la función general que al pasar por el submit valida los datos ingresados, primero comprueba que todos los datos sean diferentes de vacío para pasar, esto lo hacemos realizando un recorrido de los elementos que tiene el formulario con un bucle for y preguntando si son de tipo text, luego si pasa eso me devuelve una variable si es falso y me pinta de rojo el borde y me dice el error que tengo, para facilidad del usuario del sistema.
Luego en otro if llamo al método siguiente para validar la cedula, si me devuelve true pasa el requisito, luego el correo y la fecha de nacimiento, se declaro una variable para cada una de estas preguntas de tipo boolean que inician en false, a excepción de una que inicia en true, que se vuelve falsa si algún input este vacío y no deja enviar el formulario.
Cada una de las preguntas que se hacen con los if devuelve un valor true si se cumple y al final pregunta si todas son true la general se vuelve true y se retorna para que se envíen los datos por el formulario.
 
El método de aquí sirve para validar ya sea los nombres o apellidos, como pide el trabajo, primero recibe el objeto que lo llama, obtiene el valor del input y pregunta si es Nombre o Apellido, luego cada carácter lo convierte a ASCII para facilitar la pregunta de si son letras, si cumple estos ingresa y divide el contenido con split, para saber si hay dos palabras, si supera las dos palabras da error de que no cumple con los requisitos, y si un carácter no pertenece a los que se permiten se borra automáticamente, esto aplica tanto para Nombre y Apellidos.
 
 
 
Ahora validamos la fecha, con ayuda de la función substr(), cortamos los datos necesarios como son día, mes y año, primero validamos con ayuda de ifs que los días sean los permitidos, según el mes y según el año si es bisiesto.
Luego validamos si el día que ingresamos es mayor al día actual, seguido de el formato, que no es mas que preguntar si los símbolos slash están donde es su lugar, si cumple las validaciones se hacen true, por una falsa ya no la acepta, caso contrario si todo va bien retorna un true que nos sirve en la función general.
 
Ahora validamos el teléfono, que así mismo recibe el elemento de donde se llama al método. Se obtiene el valor del input en una variable, que luego cada carácter se pasa a ASCII para facilitar las preguntas en el if, si cumple pasa y pregunta si es mayor a 10 el numero se pinta de rojo el input en cuestión, si no pertenecen los caracteres ingresados a los permitidos se borran automáticamente en tiempo real.
 
 
Aquí le pasamos el valor del elemento desde la función general, luego preguntamos si es igual a 10 la longitud desarrollamos la comprobación de la cédula ecuatoriana, multiplicamos por 2 los números en posiciones pares y por uno en posiciones impares, si la multiplicación por 2 es mayor a 9 se le resta 9 y luego se hace una suma de estos nuevos valores, luego el valor de la suma lo subo al inmediato superior, y restamos el valor de la suma de su inmediato superior y si este numero es igual al ultimo digito se valida como true.
 
 
Ahora para validar el correo, al método le pasos el id del elemento, luego con ese obtenemos el valor del input y preguntamos si es menor o igual a 70 lo validamos, si lo es obtenemos su última parte según la validación ya sea @ups.edu.ec o @est.ups.edu.ec, luego preguntamos si lo obtenido es igual a lo inicial y si es mayor o igual a 14 en el caso de @ups.edu.ec o en el else si es mayor o igual a 18 e igual a @est.ups.edu.ec, si cumple esto, para cada caso recorreremos el valor de input y preguntaremos si hay mínimo 3 caracteres antes de las terminaciones requeridas y con ASCII validamos in son caracteres alfanuméricos.
Y si cumple retornara un true.

Commit y Push
 
 



3.	Galería
Diseñar una interfaz en html que tenga tres botones que diga “Anterior”, “Iniciar”, “Siguiente”, y una imagen. Luego, desde javascript se debe controlar para al hacer clic sobre uno de los botones realice una acción relacionada a una galería de imágenes (ver ejemplo, https://gihp4c.blog.ups.edu.ec/)
Indicaciones:
• Se debe tener, un arreglo con los nombres de diez imágenes, previamente descargadas y almacenadas en una carpeta llamada “imagen”.
• La galería de imágenes debe visualizar exclusivamente 5 imágenes. 
• Cada vez que se haga clic en el botón iniciar se deben escoger de manera aleatoria cinco imágenes de las diez que se mostrarán en la galería de imágenes.
• Al hacer clic en el botón siguiente y haber llegado a la última imagen disponible, el botón siguiente deberá ser deshabilitado (sólo cuando se ha llegado a la última imagen el botón siguiente deberá estar deshabilitado)
• Al hacer clic en el botón anterior y haber llegado a la primera imagen disponible, el botón anterior deberá ser deshabilitado (sólo cuando se ha llegado a la última imagen y cuando se inicie la galería de imágenes el botón anterior deberá estar deshabilitado)

HTML5
 
Aquí tenemos el archivo .html que se llama index, donde tenemos escritas las etiquetas necesarias para nuestra actividad, como dije anteriormente en la etiqueta head se importa tanto el archivo .css como .js para que funcione la actividad.
En el body tenemos, una etiqueta para el título, la etiqueta img para visualizar la imagen dentro de una etqieuta center para alinear al centro, así mismo dentro de otra etiqueta center tenemos los inputs para los botones de Anterior, Iniciar, Siguiente alineados al centro.

Para llamar al método tenemos el evento onload para cuando se cargue el body se visualize las 5 imágenes seleccionadas aleatoriamente, caso contrario si quiero diferente imágenes hacemos click en iniciar y cambiaran, los botones cada uno lleva un evento de onclick.
CSS3
 
No es mucho uso de reglas css, solo una para las imágenes, el color de fondo del body y otra para los input, los botones.

JAVASCRIPT
 
Como pide el trabajo esta declarado el arreglo con el nombre de las fotos, el nuevo arreglo para las fotos aleatorias resultantes, y la posición para el uso de los botones.

La función init() se encarga de cuando el body cargue, la posición es 0, llame al método iniciar() para que se carguen 5 imágenes aleatorias, show() para mostrar la imagen en la posición 0  del arreglo y loc() para validar donde estamos y así saber cuándo deshabilitar los botones que lo requieran.

La función loc() se encarga de identificar el lugar en donde nos encontramos, si es 0 deshabilita el botón Anterior, si esta entre 0 y 4 , ambos están deshabilitados y si está en la posición 4 deshabilita el botón Siguiente.

La función anterior() se encarga de hacer que se retroceda, restándole 1 a la posición actual, llamando al método loc() para saber dónde estamos y al método show() para mostrar la imagen.
 
La función iniciar() carga las 5 imágenes aleatorias tomadas del arreglo principal, como lo dice su nombre inicar, la posición se vuelve a cero, llama al método loc() para saber la ubicación, luego recorre un bucle para darle los valores de las imágenes aleatorias a un nuevo arreglo con el cual se trabaja, ahí crea un numero aleatorio entre 0 y 9, los cuales representan la ubicación de las fotos aleatorias escogidas del arreglo principal, luego un while pregunta si el valor obtenido ya se encuentra en el arreglo, si lo esta calcula de nuevo hasta obtener uno diferente, luego le damos al nuevo arreglo el valor obtenido del arreglo general en la posición que nos da el aleatorio y finalmente muestra la imagen, según lo obtenido.
La función show() se encarga de mostrar la imagen según el valor del arreglo.
La función siguiente() se encarga de hacer que se vaya hacia adelante, sumándole 1 a la posición actual, llamando al método loc() para saber dónde estamos y al método show() para mostrar la imagen.

Commit y Push
 
 
4. Luego, se debe crear el archivo README del repositorio de GitHub. 
 
5. Información de GitHub (usuario y URL del repositorio de la práctica).
Usuario: jmurillov1
URL del repositorio: https://github.com/jmurillov1/Practica03-Javascript

6. En el archivo README del repositorio debe constar la misma información del informe de resultados de la práctica que se indica en el siguiente punto. 



RESULTADO(S) OBTENIDO(S):
•	Tener el conocimiento suficiente para que el estudiante pueda entender y organizar de una mejor manera los sitios de web y de negocios en Internet.
•	Tener el conocimiento sobre nuevas etiquetas y su uso.
•	Aprender a usar HTML5 y CCS3.
Resultados:
Sitio Web Completo: Google Chrome
1.Calculadora
 
   
2. Validaciones
 
Campos Vacios
 
Valores Falsos
 
Todo bien.
3.Galeria
 
Sitio Web Completo: Firefox
1. Calculadora
     
2. Validaciones
 
 
3. Galería
 









Sitio Web Completo: Internet Explorer
1. Calculadora
 
 
 
2. Validaciones
   









3. Galería
 
CONCLUSIONES:
•	Los estudiantes podrán organizar sitios web basados en el lenguaje de etiquetado HTML, CSS y JavaScript.
•	Que el uso de JavaScript juntamente con HTML y CSS ayuda mucho a desarrollar de mejor forma los sitios web.
RECOMENDACIONES:
•	Probar la solución de la práctica en al menos tres navegadores web; Google Chrome, Firefox y Safari.
•	Validar las páginas creadas con un software, como es el caso de: W3C Validator.
•	Usar correctamente las etiquetas HTML y las formas de CSS y el código para JavaScript.

Nombre del estudiante: Jordan Fernando Murillo Valarezo

Firma del estudiante: Jordan Murillo
