# Puzzle UT2 · Pieza 02: CPU: rendimiento y modelos

**Grupo:** Iván Jelti Roldán (@IvanJelti) · Nombre Clemente Gallego Pérez (@Clemente311)

## 1. Qué es y qué función cumple en el sistema

- El funcionamiento de la CPU (Central Processing Unit) requiere de que se repita billones de veces por segundo estos tres pasos conocidos  como Fetch, Dec>
	- Fetch o Buscar: El procesador  busca y obtiene la instrucción que viene desde la memoria.
	- Decode o Decodificar: El procesador decodifica la información que ahora posee para poder entender qué tiene que hacer a partir de ese momento.
	- Excute o Ejecutar: Una vez que el procesador entiende qué tiene que hacer, lo hace. A partir de ese momento manda instrucciones al resto de los componen>

## 2. Cómo funciona por dentro

[La CPU por dentro](img/Interior_CPU.jpg)
[Presentación](img/Presentacion_Interior_CPU.pdf)

## 3. Características, unidades y cómo se miden

| Característica | Unidad | Valores típicos hoy | Qué significa |
|---|---|---|---|
| Frecuencia | GHz | Entre 3 y 6 GHz | Indica los ciclos de reloj por segundo, no las instrucciones. |
| Núcleos | Número | Entre 4 y 16 | Unidades que permiten repartir el trabajo. |
| Hilos | Número | Entre 8 y 32 | Tareas de ejecución que puede gestionar la CPU. |
| Caché | MB | Desde pocos MB hasta más de 100 MB | Memoria rápida que ayuda al procesador. |
| TDP | W | Entre 65 y 200 W | Referencia para elegir la refrigeración; no es un consumo fijo. |
| Fabricación | nm | Por ejemplo, 4, 5 o 6 nm | Identifica la tecnología usada para fabricar el chip. |
| Arquitectura | Sin unidad | x86-64 o ARM64 | Indica qué instrucciones entiende. |
| Socket | Sin unidad | AM5 o LGA1851 | Conexión de la CPU con la placa base. |
| RAM compatible | Tipo y MT/s | DDR5, por ejemplo a 5600 MT/s | Indica qué memoria puede utilizar y su velocidad de transferencia. |

Los valores son orientativos para procesadores de sobremesa; cambian según el modelo.

## 4. Tipos, evolución y estándares actuales

**Tipos**
- En el mundo de los procesadores existen varios tipos siendo uno de ellos la CPU  y se pueden organizar de la siguiente manera:

- **APU:** La Accelerated Processing Unit es un chip "dos en uno" que combina un procesador tradicional (CPU) y una tarjeta gráfica (GPU) en una sola pieza.
- **NPU:** La Neural Processing Unit es un microchip especializado en ejecutar tareas de inteligencia artificial (IA).
- **CPU:**  La Central Processing Unit ha sido ya explicada anteriormente pero os vamos a explicar cómo se estructuran sus modelos según su fabricante y gama principal. Intel (I), AMD (RYZEN).
	
	- (i3 / Ryzen 3): Perfecto para el ámbito académico, trabajo de oficina y contenido multimedia ligero.
	- (i5 / Ryzen 5): Gama media, equilibrado para gaming moderado y multitarea.
	- (i7 / Ryzen 7): Gama alta, para juegos exigentes, edición de vídeo en 4K y diseño.
	- (i9 / Ryzen 9): Gama máxima o entusiasta; para producción audiovisual pesada, modelado 3D y cargas de trabajo extremas.
- Intel
	- Intel Core Ultra: Nuevas generaciones enfocadas en eficiencia e integración de Inteligencia Artificial (NPU).
	- Intel Xeon: Diseñados para servidores y estaciones de trabajo profesionales que funcionan de forma continua.
- AMD
	- Athlon: Gama de entrada para tareas domésticas sencillas.
	- Threadripper: Los procesadores AMD Ryzen Threadripper están pensados para estaciones de trabajo profesionales y entusiastas extremos, un ámbito donde un PC normal se queda corto, pero no se necesita un servidor de empresa. La gama EPYC de este tipo de procesador está orientada a servidores y centros de datos.

**SoC:** Es un circuito integrado que contiene todos o casi todos los componentes de un ordenador en un mismo sitio. Un buena comparación entre CPU y SoC seria Apple con sus series M y A que se explican de la siguiente forma:

	* La serie M (M1, M2, M3, M4 y sus variantes Pro, Max y Ultra): Son procesadores exclusivos de los ordenadores Mac, y destacan por su altísima eficiencia energética y potencia integrada.
	* La serie A(A18, 19 Pro, 20): Son procesadores específicamente para dispositivos móviles (iPhone y los modelos base de iPad). Priorizan una eficiencia térmica extrema y el ahorro de batería.

**Evolución**
- La evolución de la CPU se resume en hacer los procesadores cada vez más pequeños, rápidos y eficientes a lo largo de cuatro grandes saltos tecnológicos:

	- Tubos de vacío (años 40): Eran máquinas gigantescas que ocupaban habitaciones enteras y consumían muchísima electricidad.
	- Transistores y microchips (años 50-70): Se redujo drásticamente el tamaño, culminando en 1971 con el Intel 4004, el primer microprocesador en un solo chip de silicio.
	- Salto a los 32/64 bits y multinúcleo (años 80-2000): Aumentó la capacidad de procesar datos y se empezaron a poner varios núcleos dentro de un mismo chip para hacer varias tareas a la vez.
	- Miniaturización e IA (2010-Presente): Hoy tienen miles de millones de transistores microscópicos, consumen muy poca batería (como en los móviles) e incluyen piezas especiales para acelerar la Inteligencia Artificial.

**Estándares actuales**
- En los PC de sobremesa modernos con Sockets AM5 en AMD o LGA1851 en Intel, destacan la memoria DDR5 y las conexiones PCIe 5.0 para GPU y SSD

## 5. Un modelo real: ficha técnica interpretada

**Modelo:** AMD Ryzen 7 9800x3d [AMD Ryzen 7 9800x3d](https://www.amd.com/en/products/processors/desktops/ryzen/9000-series/amd-ryzen-7-9800x3d.html#product-specifications)

| Dato de la ficha | Qué significa | ¿Es bueno? | ¿Para qué uso? |
|---|---|---|---|
| 8 núcleos | Puede repartir el trabajo entre 8 unidades de procesamiento. | Sí, buena cantidad para jugar y trabajar. | Juegos, programación y multitarea. |
| 16 hilos | Permite gestionar más tareas a la vez. | Sí, mejora el aprovechamiento de los núcleos. | Tener varios programas abiertos y realizar trabajos exigentes. |
| Frecuencia: 4,7 GHz, hasta 5,2 GHz | Indica los ciclos de reloj por segundo. Puede aumentar la velocidad cuando hace falta. | Sí, aunque los GHz no lo dicen todo. | Juegos y aplicaciones que necesitan rapidez. |
| Caché L3: 96 MB | Memoria muy rápida que guarda datos cerca de los núcleos. | Sí, es uno de sus puntos fuertes. | Especialmente juegos. |
| Arquitectura Zen 5 | Es el diseño interno de sus núcleos. | Sí, es una arquitectura moderna. | Juegos y trabajo general. |
| TDP: 120 W | Referencia para calcular la refrigeración necesaria; no es un consumo fijo. | Necesita buena refrigeración. | Elegir un disipador adecuado. |
| Socket AM5 | Es la conexión del procesador con la placa base. | Sí, pero requiere una placa compatible. | Montar o actualizar el ordenador. |
| Memoria DDR5 | Es el tipo de RAM que utiliza. | Sí, pero no admite DDR4. | Juegos y programas actuales. |
| PCIe 5.0 | Conexión de alta velocidad para componentes. | Sí, ofrece mucho ancho de banda. | Tarjetas gráficas y SSD compatibles. |
| Gráficos integrados básicos | Puede dar imagen sin una tarjeta gráfica dedicada. | Bien para tareas sencillas, no para juegos exigentes. | Ofimática y diagnóstico del equipo. |
| Disipador no incluido | La refrigeración se compra aparte. | Hay que contar con ese gasto. | Completar el montaje del ordenador. |

[Ryzen 7 9800x3d](/img/Encapsulado_Ryzen7_9800x3d.jpg) [Caja Ryzen 7 9800x3d](/img/Caja_Ryzen7_9800x3d.jpg)

## 6. Averías típicas y errores al elegirla o instalarla

- Un fallo de arranque o un bloqueo no significa necesariamente que la CPU esté averiada: también puede deberse a la BIOS, la RAM o el montaje.

| Problema o error | Qué ocurre | Cómo evitarlo o solucionarlo |
|---|---|---|
| Elegir componentes incompatibles | El procesador necesita una placa AM5 y memoria DDR5; no sirve para una placa AM4 ni para RAM DDR4. | Comprobar la lista de CPU compatibles y la memoria admitida por la placa antes de comprar. |
| BIOS sin soporte para el procesador | El ordenador puede encenderse, pero no arrancar correctamente. | Comprobar la versión de BIOS necesaria y actualizar siguiendo las instrucciones del fabricante. |
| Refrigeración insuficiente o mal montada | La CPU puede calentarse demasiado y reducir su rendimiento. | Utilizar un disipador adecuado, comprobar la pasta térmica y revisar el montaje y los ventiladores. |
| Colocar mal la CPU o forzar el montaje | Puede provocar daños físicos o fallos de funcionamiento. | Respetar la orientación indicada y seguir el manual, sin forzar el procesador ni el mecanismo de cierre. |
| RAM mal instalada o configuración inestable | Pueden aparecer bloqueos, reinicios o ausencia de imagen. | Colocar los módulos en las ranuras recomendadas y probar con los ajustes predeterminados de la BIOS. |
| Ajustes de overclocking inestables | El equipo puede fallar aunque los componentes estén en buen estado. | Volver a los valores predeterminados antes de diagnosticar una avería. |
| Comprar la CPU sin contar con la refrigeración | El Ryzen 7 9800X3D no incluye disipador. | Incluir un sistema de refrigeración compatible en el presupuesto. |

- La **prevención** más importante es comprobar la compatibilidad antes de comprar y seguir los manuales de la placa base y del disipador durante el montaje.

## 7. Fuentes

[Fuentes](/img/CPU_FUENTES.pdf)


## Uso de IA

- Para compararlo con otra CPU de sobremesa, elijo el Ryzen 9 9950X: entre ambos, es la opción más recomendable para trabajos de IA que aprovechan muchos núcleos. El Ryzen 7 9800X3D está especialmente orientado a juegos. Esto no significa que el 9950X sea más rápido en todas las aplicaciones de IA.

### Comparación sencilla

| Característica | Ryzen 7 9800X3D | Ryzen 9 9950X |
|---|---|---|
| Núcleos e hilos | 8 núcleos y 16 hilos | 16 núcleos y 32 hilos |
| Frecuencia máxima | Hasta 5,2 GHz | Hasta 5,7 GHz |
| Caché total L2 + L3 | 104 MB | 80 MB |
| TDP | 120 W | 170 W |
| Principal ventaja | Gran caché, especialmente útil en juegos | Más núcleos para repartir trabajos exigentes |

### ¿Cuál elegir para IA?

- Ryzen 9 9950X: lo elegiría para preparar datos, ejecutar varias tareas y trabajar con programas de IA que aprovechen sus 16 núcleos. La ventaja depende del programa y del modelo utilizado; no se puede deducir una mejora exacta solo por tener el doble de núcleos.
- Ryzen 7 9800X3D: lo elegiría si la prioridad es jugar y la IA es un uso secundario. Su caché adicional no garantiza que supere al 9950X en IA.

- Para entrenar modelos grandes o ejecutar cargas intensivas, la GPU y su memoria suelen ser más importantes que elegir entre estas dos CPU.

- Si utilizas ChatGPT u otra IA alojada en la nube, el procesamiento del modelo se realiza en servidores, por lo que no necesitas cambiar el procesador para usarla. La elección del hardware depende de dónde y cómo se ejecute la IA.

[Ryzen 7 9800x3d](/img/DIE_Ryzen7_9800x3d.png) [Ryzen 7 9950X](/img/DIE_Ryzen9_9950X.png)
