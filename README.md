# Aprendizaje Reforzado: Atari

Repositorio creado por *Juan Felipe Osorio Ramírez* durante el curso de Minería de Datos en la Universidad Nacional de Colombia, Sede Bogotá.

El contenido (imágenes, teoría y código) se toma de las siguientes referencias y tiene con último fin la **academia**:

0. [Montenegro, Álvaro. Curso en Ciencia de Datos](https://github.com/AprendizajeProfundo/Ciencia-de-Datos)
1. Saito, S., Wenzhuo, Y., & Shanmugamani, R. (2018). Python Reinforcement Learning Projects: Eight hands-on projects exploring reinforcement learning algorithms using TensorFlow. Packt Publishing Ltd.

2. Evans, L. C. (1983). An introduction to mathematical optimal control theory version 0.2. Lecture notes available at http://math.berkeley.edu/~evans/control.course.pdf .

3. Sutton, R. S., & Barto, A. G. (1998). Introduction to reinforcement learning (Vol. 135). Cambridge: MIT press.

4. Balakrishnan, K. (2020). TensorFlow Reinforcement Learning Quick Start Guide. Packt Publishing Ltd.

### Sobre las Dependencias

Este proyecto requiere el uso del lenguaje **Python** y las siguientes librerías de instaladas:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [TensorFlow1x](https://www.tensorflow.org/install/pip)

También se requiere tener algún software para correr y ejecutar un [Jupyter Notebook](http://ipython.org/notebook.html)

Si no se cuenta con Python instalado, se recomienda instalar la distribución [Anaconda](http://continuum.io/downloads) de Python, la cuál incluye muchos de los paquetes que se requieren para este proyecto y más... 

### Sobre el Código

Existe una introducción teórica al desarrollo del algoritmo junto con la explicación detallada del código del algoritmo en el cuaderno `Atari.pynb`. Y el código para entrenar el agente se concentra en los siguientes tres scripts

- `model.py` 
- `funcs.py`
- `dqn.py`

### Sobre la corrida

En una terminal o ventana de comandos, navegue hasta el directorio en el que se clonó este proyecto y corra el siguiente comando:

```bash
python dqn.py
```  
Esto correrá el script `dqn.py` el cuál llamará los otros módulos `model.py` que contiene la creación de la red neuronal y `funcs.py` que organiza el pipeline de entrada del algoritmo.

### Datos de aprendizaje

En el contexto del aprendizaje reforzado se deberán tener en cuenta las características del ambiente para entrenar nuestro agente. En particular usando los ambientes disponibles en [gym](https://gym.openai.com/envs/Breakout-v0/). Se elige el siguiente

#### Breakout-v0

En este entorno, la observación es una imagen RGB de la pantalla, que es una matriz de formas (210, 160, 3). Cada acción se realiza repetidamente durante una duración de $k$ fotogramas, donde $k$ se muestrea de manera uniforme desde $\{2, 3 , 4 \}$.

### ¡ Que empiece la diversión !
