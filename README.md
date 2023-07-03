# Integrate and Fire Neuron

The code in this repository simulates an Integrate-and-Fire neuron. A description of the model can be found in this [blog post](https://www.fabriziomusacchio.com/blog/2023-07-03-integrate_and_fire_model/).

I used  a basic Euler method for numerical integration, which might not be accurate for large time steps or fast dynamics. For a more accurate simulation, you might want to use a more sophisticated method like Runge-Kutta or use a library like [*Brian2*](https://briansimulator.org) that is specifically designed for simulating spiking neural networks.

The code is implemented in an interactive *Jupyter* notebook and you can change the parameters of model using sliders. You can run the notebook in *Google Colab* or *Binder* by clicking on onf of the buttons below:



[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/FabrizioMusacchio/integrate_and_fire_model/blob/master/integrate_and_fire_model.ipynb)   [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/FabrizioMusacchio/integrate_and_fire_model/HEAD)


Or download the notebook from this repository and run it locally.


The code models a single Integrate-and-Fire neuron for different input currents $I(t)$. First,  a the membrane potential $U(t)$ and corresponding spike times are calculated using the equation for a constant input current $I(t) = I_0$. You can interactively adjust the parameters of the model using the sliders, namely $I_0$, the resistance $R$, the capacity $C$, the firing threshold $theta§$ and the resting potential $U_\text{rest}$:


[![png](/images/integrate_and_fire_neuron_python_1.gif "Integrate-and-Fire neuron using a constant input current.")](/images/integrate_and_fire_neuron_python_1.gif "Integrate-and-Fire neuron using a constant input current.")



Second,  a the membrane potential $U(t)$ and corresponding spike times are calculated using the equation for a time-variable input current $I(t)$. Here, you can additionally adjust the membrane time constant $\tau$:

[![png](/images/integrate_and_fire_neuron_python_2.gif "Integrate-and-Fire neuron using a time-dependent input current.")](/images/integrate_and_fire_neuron_python_2.gif "Integrate-and-Fire neuron using a time-dependent input current.")



Third, a the membrane potential $U(t)$ and corresponding spike times are calculated for two input constant currents $I_{0,1}$ and $I_{0,2}$:


[![png](/images/integrate_and_fire_neuron_python_6.gif "Integrate-and-Fire neuron using two constant input currents.")](/images/integrate_and_fire_neuron_python_6.gif "Integrate-and-Fire neuron using two constant input currents.")



Simulating input currents with different intensities and durations:
[![png](/images/integrate_and_fire_neuron_python_6.png "Simulating input currents with different intensities and durations.")](/images/integrate_and_fire_neuron_python_6.png "Simulating input currents with different intensities and durations.")





Please feel free to use the code for your own projects. If you find a bug or have a suggestion for improvement, please open an issue or send me an email. 


If you use the code in your own projects, please cite it using the citation information:

> Musacchio (2023), The Integrate and Fire Model: A simple neuronal model, https://www.fabriziomusacchio.com/blog/2023-07-03-integrate_and_fire_model/

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

