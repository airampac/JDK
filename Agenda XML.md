Agenda en XML

Para hacer la agenda XML debemos seguir una estructura en este caso sera ``<agenda>`` dentro del mismo añadiremos el resto de atributos que formaran nuestro XML.
Siempre que se abre una etiqueta debemos cerrarla al terminar la información que queremos mostrar. ``</agenda>``

![1](https://user-images.githubusercontent.com/61906112/135257763-1d9f79b9-89d5-42e7-98cc-7398299b7965.PNG)


Como se puede apreciar en la imagen superior nuestro siguiente etiqueta sera ``<personas> </personas>`` y dentro de la misma añadiremos luego cada contacto o cada usuario con su información personal manteniendo asi todo agrupado y ordenado.

![2](https://user-images.githubusercontent.com/61906112/135257768-4f68f16f-4684-4fb7-8a3e-5bb894e65d46.PNG)


Dentro de personas crearemos ahora nuestros contactos cada uno con sus propios datos usando la etiqueta ``<contacto> </contacto>``

![3](https://user-images.githubusercontent.com/61906112/135257770-3bcefac5-5db4-4ba8-a508-1fc99c4dca08.PNG)


A continuación tenemos que añadir los teléfonos de nuestros contactos, es común hoy en día tener el teléfono fijo y el personal o móvil en este caso crearemos la etiqueta ``<telefono>`` y dentro de la misma,  ``<personal>``, ademas la del teléfono del domicilio con la etiqueta ``<fijo>`` y por si fuera necesario en algún caso la etiqueta ``<trabajo>``

![4 0](https://user-images.githubusercontent.com/61906112/135257776-4cf614e6-7a83-4332-8570-1258e81d095b.PNG)


Por ultimo necesitamos la dirección de cada contacto y tenerlo todo mas ordenado de la misma forma que en teléfonos creamos la etiqueta ``<dirección>`` para crear un grupo dentro de contacto, y dentro de la misma añadiremos ``<ubicación>`` para poner la calle, avenida,etc., seguido de el número del domicilio y el piso con la etiqueta`` <numero>``, para completar la dirección añadimos la etiqueta ``<poblacion>`` y por ultimo la etiqueta ``<ciudad>`` que como su propio nombre indica es para adjuntar la ciudad.

![5](https://user-images.githubusercontent.com/61906112/135257788-f3125bc1-e3ca-4a3f-9c4b-b51fa8843924.PNG)


El resultado final de nuestra agenda sera algo así, añadiendo tantos contactos como fuera necesario, siempre manteniendo el mismo orden y las mismas etiquetas.

![final](https://user-images.githubusercontent.com/61906112/135257798-d477e391-6002-4d15-bcae-9dbba94cdeb7.PNG)
