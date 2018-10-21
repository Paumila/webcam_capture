# webcam_capture

Descargar OpenCV en cas de no disposar d'ell mirjançant la següent comanda

Terminal:

pau@pau-LIFEBOOK-T904:~ $ sudo apt-get install libopencv-dev

Un cop descargada la llibreria OpenCV entrem en el nostre Github i fem un "fork" d'aquest Github https://github.com/beta-robots/webcam_capture.git

En aquest moment crea un repositori en el teu Github d'aquest webcam_capture (webcam_capture es un repositori que correspon al Github d'una altre persona)

Clonem aquest repositori que hem copiat "webcam_capture" a la carpeta que nosaltres volguem del nostre ordinador

pau@pau-LIFEBOOK-T904:~ Escritorio/Master en Robotica/Robotics Integration/repo_paumila$ git clone https://github.com/Paumila/webcam_capture.git
Clonando en 'webcam_capture'...
remote: Enumerating objects: 62, done.
remote: Total 62 (delta 0), reused 0 (delta 0), pack-reused 62
Desempaquetando objetos: 100% (62/62), listo.

Un cop clonat el repositori entrem dins la carpeta

pau@pau-LIFEBOOK-T904:~ Escritorio/Master en Robotica/Robotics Integration/repo_paumila$ cd webcam_capture/

Quan estem en el directori correcte creem una carpeta build i entrem dins d'ella per poder compilar el exacutable

pau@pau-LIFEBOOK-T904:~ Escritorio/Master en Robotica/Robotics Integration/repo_paumila/webcam_capture$ mkdir build && cd build

Un cop tenim creada la carpeta build i estem dins la carpeta comencem el procés de compilació

pau@pau-LIFEBOOK-T904:~ Escritorio/Master en Robotica/Robotics Integration/repo_paumila/webcam_capture/build$ cmake ..

pau@pau-LIFEBOOK-T904:~ Escritorio/Master en Robotica/Robotics Integration/repo_paumila/webcam_capture/build$ make
Scanning dependencies of target webcam_capture
[ 50%] Building CXX object CMakeFiles/webcam_capture.dir/src/webcam_capture.cpp.o
[100%] Linking CXX executable webcam_capture
[100%] Built target webcam_capture //En aquest punt ha creat el executable webcam_capture

A continuació executem el executable

pau@pau-LIFEBOOK-T904:~ Escritorio/Master en Robotica/Robotics Integration/repo_paumila/webcam_capture/build$ ./webcam_capture 
Opening video device 0

En aquest punt ens obre una finestra amb la nostre webcam

## Tips
https://wiki.archlinux.org/index.php/webcam_setup

http://www.linuxintro.org/wiki/Set_up_a_Webcam_with_Linux
