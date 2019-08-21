# Proyecto Final de Visión por Computador

![Banner](/otros/banner.jpg | width=850)

**Autor:** Jorge Saul Castillo Jaimes

**Objetivo:** Crear un sistema que permita el reconocimiento de placas de los vehículos que ingresan a los parqueaderos de la Universidad Industrial de Santander.

- **Dataset:** El dataset usado para realizar el reconocimiento de los caracteres de las placas es una mezcla entre char74k y uno elaborado utilizando las normas colombianas para las placas.
- **Método:** El método empleado en el desarrollo del sistema fue seguir la ideología de un ALPR (Captura de la imagen, RoI, Transformación de la imagen, Reconocimiento de caracteres)

========

## Códigos

Los códigos usados para el desarrollo del sistema se dividen en:

- Creación de nuevos datos del dataset: [GenerarDatosPlacas.ipynb](GenerarDatosPlacas.ipynb) Código en Python que permitió crear nuevos datos a raíz de los ya existentes. Los datos previos se guían de un [documento técnico del ministerio del transporte](PLACA UNICA NACIONAL.pdf) en donde se especifican las dimensiones de las placas así como las formas de los caracteres que le conforman.