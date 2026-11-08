# Teoría · LA CPU: COMO FUNCIONA, RENDIMIENTO Y MODELOS 

**Grupo:** Iván Jelti Roldán · Clemente Gallego Pérez

## CONCEPTOS CLAVE 

**Definición de CPU**
---------------------
La CPU (Central Processing Unit) se considera como “el cerebro de cualquier Sistema Informático”. Se encarga de buscar, decodificar y ejecutar todas las instrucciones del ordenador que se dividen en sistema operativo,  componentes y programas.

**Los núcleos y sus tipos**
---------------------------
Un núcleo es una unidad física de procesamiento dentro de la CPU. El tener varios permite ejecutar varias tareas a la vez, así los programas pueden repartir el trabajo.

 - P-cores (Performance cores o núcleos de rendimiento): están diseñados para tareas exigentes priorizando así el rendimiento, como videojuegos, edición de vídeo o programas que necesitan mucha capacidad de respuesta.
 - E-cores (Efficiency cores o núcleos de eficiencia): están diseñados para tareas más ligeras o secundarias buscando priorizar el bajo consumo en actividades del sistema y aplicaciones que no necesitan tanta potencia.

**¿Qué es un hilo?**
---------------------
Un hilo es una secuencia de instrucciones  lógicas que ejecuta el procesador. Gracias a las tecnologías multihilo podemos hacer que cada núcleo gestione más de un hilo y aproveche mejor sus recursos. 

Diferencia entre hilos y buses: los hilos es el proceso de la información a nivel lógico y los buses son los canales físicos por donde pasan las instrucciones. 

Con SMT (o Hyper-Threading en Intel), un núcleo puede gestionar varios hilos a la vez. Así aprovecha mejor sus recursos y puede aumentar el rendimiento, aunque no equivale a tener varios núcleos. 

**Cache**
----------
La caché es una memoria muy rápida situada dentro de la CPU. Guarda temporalmente los datos e instrucciones más utilizados para que el procesador no tenga que acceder constantemente a la RAM, que es mucho más lenta.

La CPU utiliza una jerarquía de memoria: primero busca los datos en la caché y, si no los encuentra, los solicita a la RAM. La  memoria caché se divide de la siguiente manera:
- Registros: son pequeñas memorias internas de muy poca capacidad donde la CPU guarda datos e instrucciones que necesita de manera inmediata.
- Caché L1, L2, L3: son memorias con una velocidad algo inferior al registro pero tienen mayor capacidad hallándose dentro de la CPU. La L1 es más veloz pero más pequeña que la L2 y la L2 con la L3 ocurre lo mismo.
- Puntero de instrucciones: señala la dirección de la siguiente instrucción a ejecutar.
- Registro de instrucciones: contiene la instrucción que la CPU está ejecutando actualmente.
- Buses: son los caminos físicos por donde pasan los datos entre la CPU, la memoria y otros componentes. Su anchura indica cuántos bits pueden transferirse en paralelo.

**¿Los GHz indican que CPU es más rápida?**
--------------------------------------------

La CPU se basa en una señal de reloj para sincronizar sus operaciones internas. El reloj genera un pulso constante a una frecuencia específica y estos ciclos de reloj coordinan las operaciones de la CPU. La velocidad del reloj se mide en hercios (Hz) y determina cuántas instrucciones puede ejecutar la CPU por segundo. Las CPU modernas tienen velocidades de reloj variables que se ajustan en función de la carga de trabajo para equilibrar el rendimiento y el consumo de energía. 1 GHz equivale a 1.000.000.000 de acciones por segundo.

La frecuencia base es la cantidad de operaciones que realiza por segundo bajo una carga normal. El turbo/boost (Intel Turbo Boost, AMD Precisión Boost) sube la frecuencia mientras haya margen térmico y de potencia para poder realizar tareas más exigentes.

**TDP**
--------

El TDP (Thermal Design Power) se muestra en vatios (W), pero no significa qué es lo que consume realmente, sino que indica la velocidad con la que genera calor un procesador.

**Litografia**
---------------

La litografía es el proceso que permite grabar los transistores de un procesador sobre una oblea de silicio mediante radiación ultravioleta. De este proceso depende directamente el rendimiento y la eficiencia energética del chip.

Los avances en la litografía permiten reducir el tamaño de los transistores aumentando la densidad por núcleo y aumentando también la memoria caché, dicho avance hace que sea posible aumentar la frecuencia y bajar el consumo en cada núcleo mejorando en gran medida el rendimiento del procesador tanto en multitarea como en tareas exigentes.

**Socket**
----------
Con el salto al empaquetado LGA (Land Grid Array) de 1718 contactos, AM5 representa la plataforma principal de AMD. Admite las familias Ryzen 7000, Ryzen 9000 (Zen 5) y está preparado para recibir la futura arquitectura Zen 6. Dejando atrás el AM4 que empleaba un formato PGA (Pin Grid Array) Esta transición permite un diseño de CPU más robusto y minimiza el riesgo de pines doblados en el montaje.

El socket LGA1851 se diseñó para la arquitectura Arrow Lake (Intel Core Ultra Serie 200), marcando el fin de la nomenclatura «Core i» .A pesar de ser iguales fisicamente a los de LGA1700, el aumento en la densidad de pines (1851 contactos frente a 1700) impide cualquier tipo de compatibilidad cruzada entre procesadores.

Ambos sockets tienen soporte DDR5 y PCIe5.0.

**x86 frente a ARM**
---------------------
x86 y ARM son arquitecturas de procesador: definen las instrucciones y reglas con las que se ejecutan los programas.

x86-64, usado principalmente en PCs con Intel o AMD, prioriza el rendimiento con mayor consumo y ofrece alta compatibilidad con juegos y software de PC. ARM64, presente en dispositivos de Apple, Qualcomm y otros fabricantes, se usa en móviles, portátiles y servidores, y destaca por su alta eficiencia energética, ideal para dispositivos con batería

Hoy la diferencia depende más del diseño de cada chip que del juego de instrucciones. El principal obstáculo de ARM en Windows sigue siendo la compatibilidad con software antiguo, que se resuelve mediante emulación, aunque con rendimiento variable.

**Compatibilidad y emulación**
-------------------------------
Los programas están diseñados para una arquitectura concreta. Si no existe versión nativa, puede requerir emulación. En Windows con ARM, muchas aplicaciones x86 funcionan así, pero el rendimiento varía y algunos programas o periféricos pueden no ser compatibles.

## Preguntas tipo test

[Preguntas CPU](https://play.kahoot.it/#/?quizId=7aebc689-41e8-42b3-be76-897f8ead83ed)


