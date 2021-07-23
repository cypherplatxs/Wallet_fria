# Wallet_fria
Cómo hacer una wallet fría en una USB Usando Tails y exodus


Que es [Tails](https://tails.boum.org/install/index.es.html) 

Ques es [Exodus](https://www.exodus.com/)


El primer paso es descargr el Iso de [Tails](https://tails.boum.org/install/index.es.html) de la pagina web oficial 

Luego descargamos [Etcher](https://www.balena.io/etcher/) | software con el que vamos a quemar la ISO de tails 

![BALENA](https://www.balena.io/static/steps-8006dca57323756b1b84fb9408742409.gif)

Despues booteamos el usb en el computador 

Entrar al bios > arranque  desde usb 

Al iniciar Tails debemos de generar una contraseña de administrador.

Configurar [persistencia]( https://tails.boum.org/install/clone/index.en.html#create-persistence)

tails > configuracion de persistencia > crear una

Seleccionar los archivos de las persistencia 

Descargamos Exodus 

el resultado de la descarga es un paquete tipo exodus-linux-x64-21.7.17.deb

Con el siguiente comando instalamos el paquete 

~~~
sudo dpkg -i exodus-linux-x64-21.7.17.deb
~~~

Para conectar nuestra wallet al blockchain necesitamos de instalar proxychain

~~~
sudo apt-get proxychains dnsutils
~~~

Para hacer el backup de nuestra wallet 

borrar lo que hay adentro de ./confing  y poner el back up del wallet 
