# Biestables/Flip-flops

[![DOI](https://zenodo.org/badge/991965324.svg)](https://doi.org/10.5281/zenodo.15535409)

Un simulador de lógica digital basado en reglas sencillas.

## Cómo funciona

En el mundo de los FlipFlop, existen 2 componentes lógicos fundamentales: los **cables** (wires), y los **flips-flops**. 
Nota: hay vamos ver sólo los tipo D.

- Los **cables** conectan los componentes y tienen un estado binario de “alimentado” o “no alimentado”. El estado de un cable se determina por las salidas de los componentes conectados: si alguna salida está alimentada, el cable estará alimentado; si todas las salidas están desalimentadas, el cable permanecerá desalimentado.  
- La salida Q negada de los  **flips-flops** son componentes con una única entrada y una única salida. Su salida es el opuesto de su entrada: si la entrada está alimentada, la salida estará desalimentada, y viceversa.  
- En la salida Q de los  **flips-flops**, su salida coincide con su entrada.

Cuando la entrada de un flip o flop cambia, su salida no se actualiza de inmediato, sino tras un breve retraso llamado **intervalo de tick**. Un **tick** es un instante en el que todas las salidas de los componentes se actualizan simultáneamente; cada componente lee el estado de sus entradas justo antes del tick, de modo que las actualizaciones dentro de un mismo tick no se afectan entre sí.

Los ticks se producen de forma periódica a una **tasa de ticks** constante. Por defecto, FlipFlop opera a **100 ticks por segundo (TPS)**, lo que equivale a un intervalo de 1/100 segundos (10 milisegundos) por tick, también denominado **MSPT** (Milliseconds Per Tick).

## Agradecimientos

Inspirado por:  
- **TUNG** y **Logic World** de Mouse Hat Games, por el estilo visual y la mecánica lógica.  
- **Minecraft** de Mojang Studios, por la construcción en cuadrícula.  
- **NandGame** de Olav Junker Kjær, por la idea de partir de algo muy simple.

## Licencia

FlipFlop se distribuye bajo los términos de la licencias **MIT**. Consulta el archivo `LICENSE` para más detalles.
