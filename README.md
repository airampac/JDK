Instalación de JDK en Linux Ubuntu) 

Vamos a proceder a instalar Java en Ubuntu, ejecutaremos la terminal de comandos de nuestra distribución de Linux, el primer paso es actualizar nuestro sistema con el comando:
```
sudo apt-get update
```


Ahora instalaremos el java con el siguiente comando: 
```
sudo apt-get install default-jdk
```


Al terminar el proceso comprobamos la instalación preguntado en el terminal que versión de java tenemos instalada.
```
java -version
```


Realizaremos el paso anterior donde instalamos el el default-jdk pero en esta ocasión con unas versiones especificas:
```
sudo apt install openjdk-11-jdk
sudo apt install openjdk-9-jdk
sudo apt install openjdk-8-jdk
```


Después de completar la instalación de la versión 8 procedemos a ejecutar el siguiente comando para ver el nombre exacto de nuestro jdk 8.


A continuación procedemos a crear las variables para ejecutar la versión 8 ya que es la que tener interés en usar:
```
export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
```

Ahora modificaremos el fichero profile con el comando nano de la siguiente manera.
```
nano etc/profile
```

y añadimos añadimos:
```
# Java version
JAVA_HOME=/usr/lib/jvm/_____openJdk_____
PATH=$PATH:$HOME/bin:$JAVA_HOME/bin
export JAVA_HOME
export JRE_HOME
export PATH
```


Para asegurarnos el uso predeterminado de la versión 8 añadiremos un ultimo comando  y seleccionaremos la version 8 con el numero que nos indique, acto seguido comprobaremos que estamos priorizando el uso de la misma.
```
Sudo update-alternatives –config java

java -version
```

