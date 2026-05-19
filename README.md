# Dataset procesado de baterías de litio para selección de atributos con algoritmos cuánticos

Este repositorio contiene un dataset procesado para experimentos de selección de atributos y clasificación mediante algoritmos híbridos clásico-cuánticos. El conjunto de datos fue construido a partir del dataset original **eVTOL Battery Dataset**, disponible públicamente en KiltHub/Figshare mediante el DOI:

https://doi.org/10.1184/R1/14226830

## Descripción general

El dataset original contiene mediciones experimentales de baterías de ion-litio sometidas a perfiles de carga y descarga asociados con ciclos de operación de aeronaves eléctricas de despegue y aterrizaje vertical, conocidas como eVTOL. A partir de dicho conjunto original, se realizó un proceso de selección, limpieza y estructuración de datos para obtener un dataset reducido y preparado para tareas de aprendizaje automático.

El dataset procesado incluido en este repositorio está compuesto por:

- **637 vectores**
- **10 atributos**
- **3 clases de clasificación**

Las clases consideradas corresponden a subconjuntos derivados de las celdas:

- `VAH10`
- `VAH25`
- `VAH30`

## Atributos del dataset

El dataset procesado contiene los siguientes atributos:

| Atributo | Descripción |
|---|---|
| `time_s` | Tiempo transcurrido del experimento, expresado en segundos. |
| `Ecell_V` | Voltaje de la celda, expresado en volts. |
| `I_mA` | Corriente registrada en la celda, expresada en miliamperes. |
| `EnergyCharge_W_h` | Energía acumulada durante el proceso de carga, expresada en watt-hora. |
| `QCharge_mA_h` | Capacidad acumulada durante la carga, expresada en miliampere-hora. |
| `EnergyDischarge_W_h` | Energía acumulada durante el proceso de descarga, expresada en watt-hora. |
| `QDischarge_mA_h` | Capacidad acumulada durante la descarga, expresada en miliampere-hora. |
| `Temperature__C` | Temperatura registrada de la celda, expresada en grados Celsius. |
| `cycleNumber` | Número de ciclo de carga/descarga. |
| `Ns` | Segmento o estado asociado al ciclo experimental. |

Además, cada registro incluye una etiqueta de clase asociada a la celda de origen: `VAH10`, `VAH25` o `VAH30`.

## Origen de los datos

Este dataset es una versión procesada y reducida construida a partir de:

**Bills, A., Viswanathan, V., Sripad, S., Frank, E., Charles, D., & Fredericks, W. L.  
eVTOL Battery Dataset. Carnegie Mellon University. KiltHub/Figshare.  
DOI: 10.1184/R1/14226830**

El dataset original no fue creado por los autores de este repositorio. Este repositorio únicamente contiene una versión procesada con fines académicos y experimentales.

## Objetivo del dataset procesado

El objetivo de este dataset es facilitar experimentos relacionados con:

- Selección de atributos.
- Reducción de dimensionalidad.
- Clasificación supervisada.
- Aprendizaje automático cuántico.
- Algoritmos híbridos clásico-cuánticos.
- Evaluación de modelos como QSVM y métodos de selección secuencial de atributos.

En particular, este dataset fue preparado para analizar el comportamiento de diferentes baterías de litio y evaluar qué atributos son más relevantes para distinguir las clases consideradas.

## Uso recomendado

Este dataset puede utilizarse para experimentos académicos relacionados con clasificación y selección de características. Se recomienda citar tanto este repositorio como el dataset original.

## Cita del dataset original

Si utilizas este dataset procesado, cita también la fuente original:

```bibtex
@misc{bills2021evtol,
  author       = {Bills, Alexander and Viswanathan, Venkatasubramanian and Sripad, Shashank and Frank, Evan and Charles, Devin and Fredericks, William Leif},
  title        = {eVTOL Battery Dataset},
  year         = {2021},
  publisher    = {Carnegie Mellon University},
  howpublished = {KiltHub/Figshare},
  doi          = {10.1184/R1/14226830},
  url          = {https://doi.org/10.1184/R1/14226830}
}
