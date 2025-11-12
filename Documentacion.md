# Proyecto final: Visión Artificial 
## Integrantes: David Galvis, Luciana Gutiérrez, Argenida Yehizabeth Pedraza
### Portales 
El proyecto puertas del tiempo es una experiencia interactiva pensada para el museo Juan del corral y el museo de Arte religioso de Santa Fe de Antioquia, la cual invita al espectador a atravesar los límites del tiempo y el espacio. Nuestro proyecto busca crear un diálogo entre el pasado y el presente, donde cada interacción abre una puerta hacia épocas clave de la historia de Santa Fe de Antioquia, permitiendo verla desde comunidades poco visualizadas.

## Etapa de Diseño

- ### Investigación y referentes
  
Durante esta etapa, visitamos los museos y conversamos con historiadores, guías y miembros de la comunidad para comprender cómo se cuenta actualmente la historia de Santa Fe de Antioquia y qué vacíos narrativos existen.

Identificamos una problemática central: la necesidad de renovar las narrativas patrimoniales mediante medios tecnológicos que conecten con el público actual.
La visión artificial se presentó como una herramienta ideal para lograr una interacción natural a través de gestos, permitiendo que el usuario explore las distintas “puertas del tiempo” sin necesidad de dispositivos físicos.

Entre los referentes conceptuales destacamos la película “Howl’s Moving Castle” (El castillo ambulante), en la que una puerta cambia de destino al girar un selector, transformándose en un portal hacia distintos lugares.
Tomamos de este referente la idea de la puerta como interfaz simbólica, conectando con la arquitectura tradicional santafereña, donde lo que  mas destca son lo conservds de sus fachadas y puertas coloniales.


<img width="853" height="480" alt="image" src="https://github.com/user-attachments/assets/7cb3a11c-550a-4d2a-8040-79e01a55292a" />
<img width="526" height="526" alt="image" src="https://github.com/user-attachments/assets/16aa4f46-fa4a-467a-b24c-e1cb5d49990f" />

    
- ### Diseño conceptual

<img width="1301" height="777" alt="image (1)" src="https://github.com/user-attachments/assets/fe4db580-17cc-4749-8051-a25ed7e78e1d" />

- ### Planificación técnica

Cada puerta representa una época o una historia específica de Santa Fe de Antioquia. por ende querimos que el usuario pudiera elegir entre las distintas puertas sin necesidad de que opriiera ningun tipo de botos o tuviera que tener una interracion tradicionl o fisica, eso nos llevo  la idea de los gestos de la mano y como los podimos usar de forma sencilla para que el usuario se moviera entre las puertas.

Al detectar un gesto de la mano, el sistema interpreta la acción como la elección de una puerta, activando su apertura y desencadenando una transición visual que transporta al espectador.

Se definieron los siguientes elementos principales del sistema:

Entrada: Gestos de la mano detectados mediante hand pose detection.Se hace mediante un algoritmo de p5.js con la librería ml5 que detecta 21 puntos de la mano y los muestra en pantalla, este mismo se encarga de detectar cuántos dedos tiene el usuario levantados.

Comunicación: Envío de los datos al servidor local (localhost) con Node.js el cual se la manda a unity.

Salida: unity se encarga de recibir los datos y accionar las puertas con cada un de las animaciones y respuesta visual donde se abren las puertas y cambia la escena.

## Etapa de Implementación

- ### Reporte de desarrollo
  En esta fase nos dimos cuenta de la importancia de testear cada módulo por separado antes de integrarlo. Varias veces los errores no estaban en el código sino en la forma en que los programas se comunicaban entre sí.

  Nos concentramos en conectar todos los componentes del sistema y comprobar que la interacción funcionara de manera fluida entre p5.js, Node.js y Unity.
Comenzamos implementando el algoritmo de detección de mano utilizando la cámara del computador A partir de esos puntos, el sistema identifica cuántos dedos tiene levantados el usuario y traduce esa información en un número que luego se usa como comando.
Una vez lograda la detección estable, configuramos el servidor en Node.js para recibir los datos desde p5.js y reenviarlos a Unity mediante WebSocket.
Durante las primeras pruebas trabajamos con videos simples o de prueba para verificar el funcionamiente y coordinacion.

- ### Integración
El proceso de integración fue gradual y requirió coordinación constante entre los tres entornos de trabajo.
Primero se probó la detección de gestos en p5.js, luego se estableció la conexión con Node.js, y finalmente la comunicación hacia Unity.

- ### Retos
  

- ### Reflexiones sobre el proceso creativo

