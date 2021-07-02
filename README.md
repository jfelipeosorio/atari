# Reinforcement Learning: Atari

This example was done by @juanosoriodata during Data Mining course at Universidad Nacional de Colombia, Bogotá.

Content (images, theory and code) is taken from the following references and it also has the academy as a distinct objective:

0. [Montenegro, Álvaro. Curso en Ciencia de Datos](https://github.com/AprendizajeProfundo/Ciencia-de-Datos)
1. Saito, S., Wenzhuo, Y., & Shanmugamani, R. (2018). Python Reinforcement Learning Projects: Eight hands-on projects exploring reinforcement learning algorithms using TensorFlow. Packt Publishing Ltd.

2. Evans, L. C. (1983). An introduction to mathematical optimal control theory version 0.2. Lecture notes available at http://math.berkeley.edu/~evans/control.course.pdf .

3. Sutton, R. S., & Barto, A. G. (1998). Introduction to reinforcement learning (Vol. 135). Cambridge: MIT press.

4. Balakrishnan, K. (2020). TensorFlow Reinforcement Learning Quick Start Guide. Packt Publishing Ltd.

### Dependencies

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [TensorFlow1x](https://www.tensorflow.org/install/pip)

### Code

There is a theoretical explanation of the algorithm along with the code in the notebook `Atari.pynb`. The code to train the agent is in the followin 3 scripts:

- `model.py` 
- `funcs.py`
- `dqn.py`

### Run

In a script, run the following bash command:

```bash
python dqn.py
```  
This will run `dqn.py` which calls `model.py` that builds the neural network and `funcs.py` that organizes the input pipeline.

### Data

Enviroment features and rules to train the agent. Specifically, look for [gym](https://gym.openai.com/envs/Breakout-v0/). For this project we chose

#### Breakout-v0

In this environment, the observation is a RGB image (210, 160, 3). Each action is performed 
repeatedly with $k$ fotograms where $k$ is randomly sapmle from $\{2, 3 , 4 \}$.

### ¡ Let's have fun !
