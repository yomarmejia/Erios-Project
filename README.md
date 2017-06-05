# Erios-Project
Erios Project, es un projecto a nivel escolar. Cual ha sido desarrollado para crear una central de videovigilnacia basada en S.O Linux y principalmente creada para que funcione en Raspbian.
Este sistema de Videovigilancia consisten en utilizar una RASPBERRY o una placa de desarrollo con sistema operativo y conectado a una WebCam crear una pequeña central casera de VideoSeguridad.

Aquí el funcionamiento sera el Siguiente:
1.-  La WebCam detecta movimiento y envia un correo electronico a l propietario con una imagen y el texto "Hay Movimiento, si deseas ver el Streaming, haz clic en la URL."
2.- Al terminar los movimientos este sincronizara nuestra cuenta GMAIL (DRIVE)  con la carpeta donde se almacenan las imagenes del momento en el que hubo el movimiento.

Este proyecto esta desarrollado para funcionar con un servicio DDNS o con un servidor VPS.

El Servicio DDNS -  (Puede ser el de menos seguridad ya que alguien con conocimientos puede acceder a los dispositivos de nuestra Red Interna.)

El Servidor VPS - (No es necesario abrir los puertos de nuestro Router para poder acceder al Streaming, creando una cuenta con un proveedor VPS 'AMAZON AWS, Google, AZURE...' )

La instalació y configuración son practicamente automatizados.

Si accedes por a un Servidor acuerdate de introducir "ssh -X  user@Dirección"
Para Descargar el paquete de instalación copia la siguiente linea en una terminal " wget https://github.com/yomarmejia/Erios-Project/raw/master/Erios-Project.zip " 

Puedes Descomprimir el contenido con la linea " unzip Erios-Project.zip " y colocalo en la Carpeta "Home" del S.O.
En una terminal ejecuta " cd ~/Erios-Project && chmod +x erios.sh  && sudo ./erios.sh "

Si deseas realizar la instalación con Servicio DDNS debes utilizar el Script de Instalación 'Erios-Project-DDNS.sh'
Si deseas realizar la instalación con Servidor VPS debes  utilizar el Script de Instalación 'Erios-Project-VPS.sh'

