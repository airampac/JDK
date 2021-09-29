Instalación de SublimeText 3 en Ubuntu.

Vamos a realizar la instalación del software SublimeText 3 en nuestro sistema Ubuntu, lo haremos con las lineas de comando que indicaremos paso a paso a continuación, las respuestas al insertar el comando deben coincidir con las capturas de pantalla que hemos realizado en el proceso:

Paso 1 

``
sudo apt-get upgrade
``

![1 upgrade](https://user-images.githubusercontent.com/61906112/135260325-00a9b0b9-ef13-4b21-98e7-4c60cea8c803.PNG)

Paso 2 

``
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
``

![2 wget](https://user-images.githubusercontent.com/61906112/135260351-8fd8ac4c-bc1a-47f3-b727-16674420ef25.PNG)

Paso 3 

``
sudo apt-get install apt-transport-https
``

![3 apt get install transport](https://user-images.githubusercontent.com/61906112/135260371-08fd6bc7-f9ff-4546-8ec3-a2e03b053972.PNG)


Paso 4 

``
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
``

![4 echo deb](https://user-images.githubusercontent.com/61906112/135260382-5ffe8913-4617-4cc5-9e50-3a622e8781a4.PNG)


Paso 5

``
sudo apt update
``

![5 apt update](https://user-images.githubusercontent.com/61906112/135260395-23f0f6fb-b3bd-44ca-a8f6-3bc5af4fd63b.PNG)

Paso 6

``
sudo apt install sublime-text
``

![6 apt install](https://user-images.githubusercontent.com/61906112/135260403-c9668286-519b-4f17-bae1-d8ce4a2d2524.PNG)


Paso 7

Accedemos a las aplicaciones pulsando el símbolo de Ubuntu en la esquina superior izquierda para buscar SublimeText y poder empezar a usarlo.
