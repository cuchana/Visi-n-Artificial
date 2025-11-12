# Proyecto final: Visión Artificial 
## Integrantes: David Galvis, Luciana Gutiérrez, Argenida Yehizabeth Pedraza
### Portales 
El proyecto puertas del tiempo es una experiencia interactiva pensada para el museo Juan del corral y el museo de Arte religioso de Santa Fe de Antioquia, la cual invita al espectador a atravesar los límites del tiempo y el espacio. Nuestro proyecto busca crear un diálogo entre el pasado y el presente, donde cada interacción abre una puerta hacia épocas clave de la historia de Santa Fe de Antioquia, permitiendo verla desde comunidades poco visualizadas.

## Etapa de Diseño

- Investigación y referentes
  
   Tras conocer el museo, sus personas, comunidad y narrativa, nos enfocamos en solucionar una problematica central que es la renovación de narrativas por medios tecnológicos, para esto investigamos historiadores y guias turisticos, como era el dia a dia en Santa Fe en la colonia
   Queremos vincular nuestro proyecto con visión artificial porque en los conceptos que aprendimos vimos una solución al tema de los gestos y la conexión con unity, con hand pose logramos hacer unos gestos bases que le envian la informacion al proyecto para poder navegar la interfaz.
  Para desarrollar este proyecto nos inspiramos en el concepto de la película Howl Moving Castle, en el cual usan una puerta que al seleccionar el destino se vuelve un portal que hace que al abrirla te lleve al lugar indicado, visualmente buscamos que sea más realista que fantastico para lograr la conexión de la experiencia con la realidad.


<img width="853" height="480" alt="image" src="https://github.com/user-attachments/assets/7cb3a11c-550a-4d2a-8040-79e01a55292a" />
<img width="526" height="526" alt="image" src="https://github.com/user-attachments/assets/16aa4f46-fa4a-467a-b24c-e1cb5d49990f" />

    
- Diseño conceptual

<img width="1301" height="777" alt="image (1)" src="https://github.com/user-attachments/assets/fe4db580-17cc-4749-8051-a25ed7e78e1d" />

- Planificación técnica

  Interacción: Se hace mediante un algoritmo de p5.js con la librería ml5 que detecta 21 puntos de la mano y los muestra en pantalla, este mismo se encarga de detectar cuántos dedos tiene el usuario levantados, le pasa la información a un localhost por node.js el cual se la manda a unity y este se encarga de recibirla y accionar las puertas.


## Etapa de Implementación

- Reporte de desarrollo

- Integración

- Retos

- Reflexiones sobre el proceso creativo

