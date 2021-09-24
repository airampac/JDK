Instalación de JDK en Linux Ubuntu) 

Vamos a proceder a instalar Java en Ubuntu, ejecutaremos la terminal de comandos de nuestra distribución de Linux, el primer paso es actualizar nuestro sistema con el comando:
```
sudo apt-get update
```
![1](https://user-images.githubusercontent.com/61906112/134668491-010f55cb-8d52-4930-b898-a6e6e3153fb6.PNG)


Ahora instalaremos el java con el siguiente comando: 
```
sudo apt-get install default-jdk
```
![2](https://user-images.githubusercontent.com/61906112/134668529-3fdc0d82-d224-4b90-abd6-ff4e0eeaf9ce.PNG)


Al terminar el proceso comprobamos la instalación preguntado en el terminal que versión de java tenemos instalada.
```
java -version
```

![3](https://user-images.githubusercontent.com/61906112/134668541-8c495601-cc22-4618-97bd-ca1e8debaf2f.PNG)

Realizaremos el paso anterior donde instalamos el el default-jdk pero en esta ocasión con unas versiones especificas:
```
sudo apt install openjdk-11-jdk
sudo apt install openjdk-9-jdk
sudo apt install openjdk-8-jdk
```
Después de completar la instalación de la versión 8 procedemos a ejecutar el siguiente comando para ver el nombre exacto de nuestro jdk 8.

![4](https://user-images.githubusercontent.com/61906112/134668626-4de10151-8341-4d49-a014-5210d9730492.PNG)


A continuación procedemos a crear las variables para ejecutar la versión 8 ya que es la que tener interés en usar:
```
export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
```
![5](https://user-images.githubusercontent.com/61906112/134668721-614ef167-5886-4af9-945b-9e3e00fbe3f9.PNG)

Ahora modificaremos el fichero profile con el comando nano de la siguiente manera.
```
nano etc/profile
```

y añadimos las siguientes lineas de codigo:
```
# Java version
JAVA_HOME=/usr/lib/jvm/_____openJdk_____
PATH=$PATH:$HOME/bin:$JAVA_HOME/bin
export JAVA_HOME
export JRE_HOME
export PATH
```
![6](https://user-images.githubusercontent.com/61906112/134668820-97bd3180-f30b-40fc-9234-6497aabd7215.PNG)


Para asegurarnos el uso predeterminado de la versión 8 añadiremos un ultimo comando  y seleccionaremos la version 8 con el numero que nos indique, acto seguido comprobaremos que estamos priorizando el uso de la misma.
```
Sudo update-alternatives –config java

java -version
```
![7](https://user-images.githubusercontent.com/61906112/134668831-273ad875-6de8-4f2e-990d-da0caf7adf98.PNG)

