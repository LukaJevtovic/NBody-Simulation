Numerical simulations are the cornerstone of "experimental" astrophysics. While there are open source codes out there that are fully optimized and incredibly efficient, such as GADGET (https://wwwmpa.mpa-garching.mpg.de/gadget4/), it is good practice to build a barebones n-body simulation yourself first, in order to understand what's really happening "under the hood" of these massive codes.

In this repository, you will find two fully commented jupyter notebooks that use Euler and Runge-Kutta 4th order methods of numerical integration to carry out a numerical simulation of our test "galaxy". If you're a beginner, it's recommended that you start from the Euler code first, and later upgrade it to RK4, as Euler integration is much more intuitive to understand from the point of approximating calculus with discrete values.

The "galaxy" that I've used was generated using the GalactICS package (https://ui.adsabs.harvard.edu/abs/2011ascl.soft09011K/abstract). It's a very simple model that contains only 400 particles. As such, it's not completely stable over longer periods, and shouldn't be used as a realistic model. However, it provides an excellent basis for testing code, as it's very computationally lightweight, while still allowing for some rudimentary data analysis and interpretation of simulation outputs.

This data analysis can be found in the jupyter notebooks, along with my comments on them, where I discuss things like energy plots, density profiles, velocity dispersions, and so on.