# Puzzle UT2 · Pieza 02: CPU: rendimiento y modelos

**Grupo:** Iván Jelti Roldán (@IvanJelti) · Nombre Clemente Gallego Pérez (@Clemente311)

> Máximo 2 folios por las dos caras (unas 1.600–2.000 palabras) y al menos 3 imágenes en `img/`.

## 1. Qué es y qué función cumple en el sistema

- La CPU (Central Processing Unit) se considera como “el cerebro de cualquier Sistema Informático”. Se encarga de buscar, decodificar y ejecutar todas las instrucciones del ordenador que se dividen en sistema operativo,  componentes y programas.

## 2. Cómo funciona por dentro

![Esquema de funcionamiento](img/ejemplo-esquema.svg)

<!-- Guardad vuestras imágenes en img/ y cambiad el nombre del archivo en la línea de arriba. -->

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
- Las CPU pueden clasificarse por su uso: sobremesa, portátiles y servidores. También por su arquitectura: x86-64, habitual en Intel y AMD, y ARM64, utilizada por Apple, Qualcomm y otros fabricantes.

**Evolución**
- Han pasado de tener un solo núcleo a incorporar varios. La mejora ya no consiste solo en aumentar los GHz: también se busca ejecutar más tareas a la vez, ampliar la caché y reducir el consumo. Algunos diseños combinan núcleos de rendimiento y de eficiencia, como los P-cores y E-cores de Intel.

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

<!-- Aquí va la foto o captura del modelo: ![Foto del modelo](img/modelo.jpg) -->

## 6. Averías típicas y errores al elegirla o instalarla

## 7. Fuentes

[Fuentes](/img/CPU_FUENTES.pdf)


## Uso de IA

Qué preguntamos a Jarvis u otra IA y cómo comprobamos sus respuestas.
