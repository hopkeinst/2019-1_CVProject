# Proyecto Final de Visión por Computador

![Banner](https://github.com/hopkeinst/2019-1_CVProject/blob/master/otros/banner.jpg)

**Autor:** Jorge Saul Castillo Jaimes

**Objetivo:** Crear un sistema que permita el reconocimiento de placas de los vehículos que ingresan a los parqueaderos de la Universidad Industrial de Santander.

- **Dataset:** El dataset usado para realizar el reconocimiento de los caracteres de las placas es una mezcla entre char74k y uno elaborado utilizando las normas colombianas para las placas.
- **Método:** El método empleado en el desarrollo del sistema fue seguir la ideología de un ALPR (Captura de la imagen, RoI, Transformación de la imagen, Reconocimiento de caracteres)

========

## Códigos

Los códigos usados para el desarrollo del sistema se dividen en:

- Creación de nuevos datos del dataset: [GenerarDatosPlacas.ipynb](https://github.com/hopkeinst/2019-1_CVProject/blob/master/GenerarDatosPlacas.ipynb) Código en Python que permitió crear nuevos datos a raíz de los ya existentes. Los datos previos se guían de un [documento técnico del ministerio del transporte](https://github.com/hopkeinst/2019-1_CVProject/blob/master/PLACA%20UNICA%20NACIONAL.pdf) en donde se especifican las dimensiones de las placas así como las formas de los caracteres que le conforman.

- Creación de un sistema para poder clasificar/identificar los caracteres que conforman la placa: [GenerarPesos_Clasificadores.ipynb](https://github.com/hopkeinst/2019-1_CVProject/blob/master/GenerarPesos_Clasificadores.ipynb) Código en Python en el cual se desarrollo una red convolucional basada en el modelo LeNet-5 para ayudara a identificar los caracteres que componían las placas; así como también su comparación respectiva frente a otros métodos como Random Forest y KNN.

- Identificación de la placa: [LecturaPlaca.ipynb](https://github.com/hopkeinst/2019-1_CVProject/blob/master/LecturaPlaca.ipynb) Código en Python principal. Es el que se encarga de obtener una imagen o video (desde el repositorio o dataset), tomar la región de interés y posteriormente adquirir los caracteres, pasarlos por la red convolucional y dar el resultado de que placa es posiblemente.

========

## Videos informativos

- Funcionamiento parcial, en Raspberry Pi3: (Video Youtube)[https://www.youtube.com/watch?v=cPiWHs5UfCQ]

- Explicación del funcionamiento del