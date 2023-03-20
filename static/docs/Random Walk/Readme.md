# Introduction

# Random Walk, Brownian Motion and Ito Process

Ito process is a continuous-time trajectory with random evolution, so non-smooth and very kinky - also has a fractal look.

- Ito process consists in fact of two parts: the drift part (deterministic evolution) and the diffusion part (where all the kinkiness and fractalness comes from).
- If Ito process does not posses the diffusion part, it just looks like a continuous smooth trajectory.
- If Ito process has only diffusion component, you won't be able to spot it i.e. when the diffusion component is present, it's hard to say whether there is a drift component or not, because of the noise diffusion provides.
- An Ito Process is a Brownian Motion with possibly non-zero mean.

A Brownian Motion is a continuous time series of random variables whose increments are i.i.d. normally distributed with 0 mean.

- It is a special case of an Ito process, and is the main building block for the diffusion component.
- Any diffusion is just a time scaled Brownian motion.
- Its increments are uncorrelated (in fact, they are independent) whereas in general Ito process there can be loads of cross-correlation happening.

A random walk is a discrete time process whose increments are +/-1 with equal probability.

- As it is discrete time process hence not comparable with Ito processes which are continuous-time things.
- Random walk must also have independent increments - that's why Brownian motion sometimes referred to as a (continuous-time) random walk.

# Variations

Levy Flight
Self Avoiding Walk
