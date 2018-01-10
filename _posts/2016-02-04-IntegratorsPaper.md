---
layout: post
title: Quaternion Variational Integrators Paper
---

I was just notified that my first journal paper, "Quaternion Variational Integrators for Spacecraft Dynamics," which was accepted for publication in the AIAA *Journal of Guidance, Control, and Dynamics* back in April of last year, will be appearing in print in the next issue. In the paper I develop special-purpose numerical integration algorithms for simulating spacecraft attitude dynamics. The algorithms are derived by discretizing [Hamilton's Principle](https://en.wikipedia.org/wiki/Hamilton%27s_principle) (also known as the "Principle of Least Action" or "Principle of Stationary Action") and have several interesting properties, including long-term energy and momentum conservation (for conservative systems). Here's a plot from a simulation of a tumbling rigid body comparing the energy drift between the [2nd order midpoint rule](https://en.wikipedia.org/wiki/Midpoint_method), [MATLAB's ODE45](http://www.mathworks.com/help/matlab/ref/ode45.html) integrator, and the variational integrator in the paper:

![EnergyError](/img/EnergyError.png)

If you're still with me after all of that jargon, you can check out the paper on the [journal's website](http://arc.aiaa.org/doi/abs/10.2514/1.G001176) or download a preprint [here](/docs/Variational_Integrator.pdf). I'm also posting MATLAB implementations of the integrators and some demos on [GitHub](https://github.com/zacmanchester/quaternion-variational-integrators).
