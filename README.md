# Orbital
This repository includes classes, which use Open Source Physics (OSP) packages, to simulate the orbits of planets. The programs calculate the force of gravity, simulate a single planet orbit, and use the simulation to prove Keplers' three laws:
* planet's orbits due to gravity are elliptical
* the period of a planet's orbit is proportional to the length of the semi-major axis of its orbit
* the 2D sector that the planet traces out, if the other planet (presumably much heavier and unmoving) is considered the origin.

The OrbitalSimulation class is the crux of this program, containing the OSP recursive DoStep function in which the planet's position and velocity is updated from every timestep. The Planet class extends the Particle class that was developed for the 2D-Motion-Simulator repository. The Vector class lays out the characeristics of a vector (direction and magnitude) and the relevant functions (adding vectors, finding its Cartesian components, etc.). The interpolation function contains the methods necessary to interpolate a function given the corresponding number of coordinate pairs to define it.
