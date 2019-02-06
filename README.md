# ace2holamundo
Es el hola mundo del arduino, se esta prendiendo y apagando el pin 13

Sistemas operatavio: ubuntu 18.01 LTS arduino IDE: 1.8.8

Instalar audino IDE en ubuntu Descargar el instalador desde https://www.arduino.cc/en/Main/Software Extraer el archivo arduino-1.8.8-linux64.tar.xz

Luego por medio de terminal ingresar a cd arduino-1.8.8-linux64/arduino-1.8.8

./install.sh

Si da los siguientes errores

Arduino:1.8.8 (Linux), Tarjeta:"Arduino/Genuino Uno" El Sketch usa 930 bytes (2%) del espacio de almacenamiento de programa. El máximo es 32256 bytes. Las variables Globales usan 9 bytes (0%) de la memoria dinámica, dejando 2039 bytes para las variables locales. El máximo es 2048 bytes. avrdude: ser_open(): can't open device "/dev/ttyUSB0": Permission denied Ha ocurrido un error mientras se enviaba el sketch Este informe podría contener más información con "Mostrar salida detallada durante la compilación" opción habilitada en Archivo -> Preferencias.

en mi caso utilice

sudo chown /dev/ttyUSB0

pero tiene verificar en que puerto USB esta conectado el arduino
