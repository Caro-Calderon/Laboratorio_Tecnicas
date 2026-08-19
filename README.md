# Laboratorio_Tecnicas

## Tabla de Contenidos
- [1. Parte 1: Compuertas Lógicas](#1-parte-1-compuertas-lógicas)
  - [Descripción](#descripción)
  - [Simulación](#simulación)
- [2. Parte 2: Detector de Primos (3 bits)](#2-parte-2-detector-de-primos-3-bits)
  - [Diseño](#diseño)
  - [Simulación](#simulación-1)
- [3. Parte 3: Sumador Completo de 1 Bit](#3-parte-3-sumador-completo-de-1-bit)
  - [Descripción](#descripción-1)
  - [Simulación](#simulación-2)
- [4. Implementación en Hardware (Tarjeta de Desarrollo)](#4-implementación-en-hardware-tarjeta-de-desarrollo)

---

**Fecha:** 19 de Agosto de 2026  
**Grupo 4:** Heidy Carolina Calderón Romero 140804

## 1. Parte 1: Compuertas Lógicas
### Descripción
Se diseñaron las compuertas NOT, AND, OR, XOR y XNOR. Se implementaron dos versiones:
1. **Estructural:** Usando primitivas de Verilog (`and`, `or`, `not`, etc.).
2. **Comportamental:** Usando operadores lógicos y `assign`.

### Simulación
A continuación se muestra la evidencia de la simulación donde se comprueba que las salidas coinciden con las tablas de verdad teóricas.

*[INSERTA AQUÍ LA CAPTURA DE PANTALLA DE LA SIMULACIÓN DE LAS COMPUERTAS]*

## 2. Parte 2: Detector de Primos (3 bits)
### Diseño
El circuito recibe un número de 3 bits (0 al 7). Los números primos en este rango son 2, 3, 5 y 7. 
Mediante un mapa de Karnaugh, se obtuvo la siguiente ecuación booleana:
`S = (~A & B) | (A & C)`

### Simulación
Se simularon las 8 combinaciones posibles. El circuito arroja `1` solo para los números 2, 3, 5 y 7.

*[INSERTA AQUÍ LA CAPTURA DE PANTALLA DE LA SIMULACIÓN DE PRIMOS]*

## 3. Parte 3: Sumador Completo de 1 Bit
### Descripción
Sumador que recibe dos bits y un acarreo de entrada (Cin), generando una suma (Sum) y un acarreo de salida (Cout).

### Simulación
Se comprobó la tabla de verdad completa (8 estados).

*[INSERTA AQUÍ LA CAPTURA DE PANTALLA DE LA SIMULACIÓN DEL SUMADOR]*

## 4. Implementación en Hardware (Tarjeta de Desarrollo)
El diseño fue compilado en **Quartus Prime**. 
- **Entradas:** Se asignaron a los switches (SW) de la tarjeta.
- **Salidas:** Se asignaron a los LEDs (LEDR / LEDG) de la tarjeta.

*[INSERTA AQUÍ UNA FOTO DE TU TARJETA FPGA EN FUNCIONAMIENTO O CAPTURA DEL PIN PLANNER DE QUARTUS]*
El diseño fue compilado en **Quartus Prime**. 
- **Entradas:** Se asignaron a los switches (SW) de la tarjeta.
- **Salidas:** Se asignaron a los LEDs (LEDR / LEDG) de la tarjeta.

*[FPGA]*
