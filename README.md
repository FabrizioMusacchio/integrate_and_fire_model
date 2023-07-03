# Integrate and Fire Neuron

The code in this repository simulates an Integrate-and-Fire neuron. A description of the model can be found in this [blog post]([#link](https://www.fabriziomusacchio.com/blog/2023-07-03-integrate-and-fire-model/)).

I used  a basic Euler method for numerical integration, which might not be accurate for large time steps or fast dynamics. For a more accurate simulation, you might want to use a more sophisticated method like Runge-Kutta or use a library like [*Brian2*](https://briansimulator.org) that is specifically designed for simulating spiking neural networks.

The code is implemented in an interactive *Jupyter* notebook and you can change the parameters of model using sliders. You can run the notebook in *Google Colab* or *Binder* by clicking on onf of the buttons below:



[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/FabrizioMusacchio/integrate_and_fire_model/blob/master/integrate_and_fire_model.ipynb)   [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mpbrucker/mpbrucker.github.io/master?filepath=assets%2Fnotebooks%2FIntegrate-and-Fire.ipynb)

Or download the notebook from this repository and run it locally.

Please feel free to use the code for your own projects. If you find a bug or have a suggestion for improvement, please open an issue or send me an email. Please cite the code as:

Musacchio (2023), The Integrate and Fire Model: A simple neuronal model, https://www.fabriziomusacchio.com/blog/2023-07-03-integrate-and-fire-model/

or

```latex
@misc{Musacchio2023,
  author = {Musacchio, Fabrizio},
  title = {The Integrate and Fire Model: A simple neuronal model},
  year = {2023},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://www.fabriziomusacchio.com/blog/2023-07-03-integrate-and-fire-model/}},
}
```

