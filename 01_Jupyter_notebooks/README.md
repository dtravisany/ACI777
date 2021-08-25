# Tutorial de Jupyter Notebook

## Introducción

El _Project Jupyter_ es un proyecto de código abierto sin fines de lucro, que nació a partir del [Proyecto IPython](https://ipython.org/) en el año 2014. Este proyecto evolucionó para respaldar la ciencia de datos interactivos y la computación científica en todos los lenguajes de programación. 
La promesa del Proyecto _Jupyter_ es que siempre será un software 100% de código abierto, de uso gratuito para todos y publicado bajo los términos libres de la [licencia BSD 3](https://opensource.org/licenses/BSD-3-Clause).

El proyecto Jupyter se desarrolla en GitHub, a través del consenso de la comunidad de Jupyter. Si necesitas mas info de la gobernanza del proyecto Jupyter puedes verlo [acá](https://github.com/jupyter/governance/blob/master/governance.md)


## Herramientas

1. [Jupyter Notebook](https://jupyter.org/) es una aplicación web de código abierto que permite crear y compartir documentos. La principal ventaja es que contienen código 'live', ecuaciones, visualizaciones y texto narrativo que complementa el código y las visualizaciones. 

Sus principales usos incluyen: 

   1. Limpieza.
   2. Transformación de datos.
   3. Simulación numérica.
   4. Modelado estadístico.
   5. Visualización de datos.
   6. Aprendizaje automático.

Actualmente es utilizado por instituciones muy prestigiosas en el mundo como:

   1. Google
   2. Microsoft
   3. IBM
   4. NASA
   5. Bloomberg
   6. O'REILLY
   
Entre otras, una lista completa la puedes ver al final de esta [página](https://jupyter.org/).

2. [JupyterLab](https://jupyter.org/) es un entorno de desarrollo interactivo basado en web para Jupyter Notebooks. JupyterLab permite configurar y organizar la interfaz de usuario para preparar una amplia gama de pipelines/workflows en ciencia de datos, informática científica y aprendizaje automático. Otra ventaja, JupyterLab es extensible y modular: se pueden generar o descargar complementos que agregan nuevos componentes y se integran con los existentes.


## Instalación

Por defecto, como vimos en la primera clase, al instalar Anaconda, Jupyter es instalado en el proceso, además de conda(Ana-"conda").

Sin embargo, se puede instalar desde:

### Instalación de JupyterLab



#### Mamba o Conda :snake:

Los gestores de paquetes de python mamba o conda

Mamba:

    mamba install -c conda-forge jupyterlab

o mediante conda:

    conda install -c conda-forge jupyterlab

:warning: Si no le interesa instalar Anaconda uno puede instalar versiones mini de mamba o conda en la [miniforja](https://github.com/conda-forge/miniforge).


#### Mediante ``pip``

``pip`` es el instalador de paquetes de python que viene por defecto. Puedes encontrar más información [acá](https://pypi.org/project/pip/)

### Instalación Jupyter-notebook

#### Instalation con mamba o conda

    mamba install -c conda-forge notebook

o con conda:
 
    conda install -c conda-forge notebook

Instalación con ``pip``

Si usted usa ``pip``, se puede instalar con la siguiente línea:

    pip install notebook

Felicitaciones :fireworks:  has instalado Jupyter Notebook!.

Para ejecutar en linux/mac abrir una terminal, para ejecutar  en windows utilizar Anaconda prompt y escribir:

    jupyter-notebook


