# Práctica 11: ANDROID Fundamentos
## Juan A. Caballero
--------------------------------------

La práctica aquí presentada se desarrolla dentro del Máster Bootcamp 4ª edición impartido por Keepcoding y corresponde a la unidad 11 del temario de dicho máster. 


NOTAS SOBRE LA PRÁCTICA
--------------------------------------
Hasta esta tarde, todo lo desarrollado para la app me funcionaba correctamente, incluso para varios dispositivos. A primera hora de esta tarde he tenido un CRASH en el ordenador y se me ha quedado todo bloqueado con la app en Visual Studio abierta y a partir de ese momento no he podido seguir desarrollando pues me daba errores muy extraños, incluso con commit anteriores de la app que funcionaban perfectamente. 

No sé si se habrá corrompido el fichero o si será un problema de mi Android Studio, creo y espero que sea esto último. He subido una copia del proyecto, la última probada. Me da como error que no encuentra un icono en métodos internos de Android Studio y da error con la "R" en rojo de recursos. 

Todo se ha producido al intentar crear un fichero java y su Layout en xml para un Adapter personalizado para personalizar las filas del List View de platos. Borré ambos ficheros luego pero sigue dando error. 


FUNCIONALIDADES IMPLEMENTADAS
--------------------------------------
La práctica es una app desarrollada para que un restaurante pueda llevar un control de las mesas y los platos que cada una pide.

La app consta de una primera pantalla que muestra un LIST VIEW con la lista de mesas. Seleccionando cualquiera de ellas nos lleva a otra pantalla con un VIEWPAGER dentro del cual se muestra la mesa seleccionada y todos los platos que ha pedido. Desplazandonos a izquierda y derecha con el dedo podemos movernos de una mesa a otra. 

Dentro del ViewPager podemos acceder mediante la opción de menú "BILL" a otra PANTALLA CON LA CUENTA de la mesa mostrando el total en euros.

Pulsando en el ViewPager la opción de menú "ADD DISH" nos lleva a otra pantalla en la que se muestra un List View con la LISTA DE PLATOS descargada de la red en formato JSON. 

Pulsando sobre un platonos abre una pantalla de VISTA EN DETALLE DEL PLATO seleccionado, con una fotos, nombre, ingredientes, precio y una caja de texto donde podemos añadir variaciones o notas del plato. Pulsando el botón "CANCEL" vuelve hacia atrás y pulsando botón "OK" añade el plato a la mesa y nos devuelva al menú anterior. 

Desde el ListView que muestra la lista de platos, la opción de menú "RETURN TABLE" nos devuelve al ViewPager mostrando la mesa en la que estamos añadiendo platos con la lista de éstos actualizada con los últimos añadidos. 


Todas estas opciones deberían funcionar perfectamente, pues a mí me han estado funcionando estos últimos días. 


OTROS
--------------------------------------
Algunas cosas no me ha dado tiempo a implementarl, aunque comentaré brevemente aquí la forma que tenía previsto hacerlo. 

La funcionalidad de Multidispositivo está a medio hacer, pues había usado un fragment para la lista de mesas y otro fragmente para el viewpager con la idea de meter ambos en una misma actividad cuando se tratara de dispositivos grandes tipo tablet, para lo que hubiera usado los Calificadores con un rango de pantalla similar al del ejemplo de clase y según el hueco en pantalla para el fragment que me interesara metería ambos fragmente un una sola actividad para dispositivos grandes o como está ahora cada fragmente con su actividad para dispositivos pequeños. 

La funcionalidad de mostar en el ListView de platos más detalles aparte del nombre, como la imagen, ingredientes y alérgenos, no me ha dado tiempo a implementarla, pues fue precisamente creando el Adaptador en un fichero Java aparte para ello con su Layout en xml lo que me dió error. Borré ambos ficheros pero siguió el error como ya dije.

Los botones Ok y Cancel no he conseguido que ocupen la mitad cada uno. Por más que he repasado el vídeo en el que lo explicas no lo consigo, supongo que algún detalle se me habrá pasado. Los he dejado así para que veas que lo he intentado hacer como tú nos explicaste. 


Para alguien que no ha programado nunca nada antes de este Bootcamp y que ni siquiera ha tenido tiempo de ver los vídeos de Android de la web de Keepcoding salvo alguos pocos días antes del curso no está mal, no pensaba hace una semana que llegaría a implementar lo ya hecho. Pero bueno, con trabajo duro todo se consigue y supongo que con un poco más de tiempo hubiera acabado el resto de funcionalidades. 

