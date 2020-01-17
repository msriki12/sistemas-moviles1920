# sistemas-moviles1920
Documentación de la práctica final de Sistemas Móviles del curso 2019/20 del alumno ricmart

Aplicación: Mi Nevera

Funcionalidad: La aplicación mi nevera se basa en una lista en la que puedes guardar platos cocinados y refrigerados de forma que en todo momento puedas consultar los platos que tienes en la nevera y de esa manera evitar que la comida se ponga mala. La aplicación permite registrar en una lista de dos columnas un nuevo plato de comida, que consta de un nombre de plato* y un alimento principal. En función del alimento principal la aplicación determina cuántos días durará el alimento en buen estado en el refrigerador. Al elegir un alimento principal, se cambia la fotografía representativa en función de éste. Además de esto, el sistema se conecta con una API REST externa* que se encarga de proporcionar información nutricional sobre el plato que se ha introducido basándose en el nombre del plato. Esta API utiliza un motor de procesamiento de lenguaje natural para deducir algunos de los aspectos del plato.

Herramientas utilizadas: 

- Intro Slider: Para realizar un pequeño tutorial a modo de introducción que se ejecuta tan sólo la primera vez que abres la aplicación, he utilizado PageViewer y he modificado el archivo Manifest para ejecutar el Slider como Main Activity la primera vez.

- Lista de alimentos: Para mostrar la lista de alimentos he utilizado CardView + RecyclerView y para guardarlos en la base de datos he utilizado la librería Room, que permite implementar una base de datos de manera muy bien estructurada.

- Análisis de datos: Para realizar las peticiones a la API REST he utilizado la libería Retrofit2, y la API utilizada es "Nutrition Analysis API" de Edamam (https://www.edamam.com/).

Funcionamiento de la aplicación:

- Para añadir alimentos a la lista, bastará con pulsar el botón con un símbolo '+' en la parte inferior derecha de la pantalla.
- Para borrar un elemento concreto, mantener pulsado sobre el alimento y se desplegará un menú contextual con la opción de borrar.
- Para borrar todos los elementos de la lista, se debe pulsar sobre el menú situado en la parte superior derecha de la barra de herramientas, y seleccionar la opción "Eliminar todos".
- Dentro de la vista de "Añadir alimento", una vez rellena la información obligatoria (Nombre del alimento), es posible guardarlo pulsando el botón de la esquina superior derecha "GUARDAR", o bien salir en cualquier momento pulsando la X de la esquina superior izquierda.
- Para editar un alimento de la lista, se debe pulsar sobre éste.

A destacar:

- Todos los iconos/imágenes que se han utilizado para realizar la aplicación (salvo las imágenes principales de la lista de comida) han sido dibujadas por mí.

Funcionalidad a añadir:

 Sistema de gestión de notificaciones que avise cuando un alimento esté a punto de ponerse malo.
