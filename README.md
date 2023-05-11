# BH-Ray-Tracer
The C++ code simulates the motion of light rays in the vicinity of a rotating (Kerr) black hole using geodesics in curved spacetime. The simulation is based on the geodesic equations, which describe how particles and light move in a curved spacetime.

The main components of the code are:

1. Include necessary libraries and declare global variables.
2. Define the initial conditions for the light ray (initial function).
3. Define the geodesic equations (geodesic function).
4. Implement the Cash-Karp Runge-Kutta method (rkck function) to solve the geodesic equations.
5. Implement the adaptive step-size control for the Runge-Kutta method (rkqs function).
6. Binary search to find the accurate position of the light ray (binarysearch function).
7. Calculate the marginally stable orbit (RMS function).
8. Implement the main function that runs the simulation, writes the results to a file, and calculates the light intensity.

The code simulates light rays coming from a camera with a 2D grid and calculates their paths as they propagate through the curved spacetime around the black hole. The simulation stops when a ray reaches the black hole, the accretion disk, or escapes to infinity. The output data is written to a file named "position.dat".

The black hole's spin is defined by the global variable a, which is the spinning parameter (a=0.9) for this code. The inclination angle is set by theta0, which is converted to radians. Various other parameters such as field of view (fov) and resolution (m) are also defined. The main function (main()) runs the simulation for each ray in the camera grid, calculating the ray's path and the light intensity.


P.S - This is just a simple ray tracer code. No fancy geodesics calculations. Will update the code and make it more robust(with all the geodesics calculations). Till then you can play around !!
