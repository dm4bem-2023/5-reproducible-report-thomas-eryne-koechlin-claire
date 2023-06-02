# Dynamic Models for Building Energy Management

Our Binder : [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dm4bem-2023/5-reproducible-report-thomas-eryne-koechlin-claire/HEAD)
Group : Claire Koechlin and Eryne Thomas

## Project sessions
1. **Model**
 - Draw the plan of a two-zone building.
 - Formulate the hypothesis for boundary conditions.
 - Chose the types of windows, doors, and walls.
 - Draw the thermal circuit:
     - temperature nodes,
     - flow-rate paths,
     - thermal conductances for conduction, convection, long-wave radiation, advection, and P-controllers,
     - sources of temperature and flow-rate,
- Number the temperature nodes and the flow-rate branches (starting from 0).
 - Calculate the thermal conductances for conduction, convection, long-wave radiation, and advection.
 - Calculate the thermal capacities.
 - Write down the incidence matrix $A$, the conductance matrix $G$ and the capacity matrix $C$ of the system of Algebraic Differential Equations (DAE).
 - Define the inputs: temperature sources (vector $b$) and flow rate sources (vector $f$).
 - Write in Pyhthon the incidence matrix $A$, the conductance matrix $G$ and the capacity matrix $C$ of the system of Algebraic Differential Equations (DAE).
 - Write in Pyhthon the vectors of pointers to the temperature sources $b$, flow-rate sources $f$, and outputs $y$.
 - **Assignment 1**: Model
     - [Grup 1, 2](https://classroom.github.com/a/Fh4jnCT2)
     - [Grup 3, 4](https://classroom.github.com/a/bl3pb-J7)
 
2. **Steady-state**
 - Implement in Python the matrices $A$, $G$ and $C$ of the system of Diferential Algebraic Equations (DAE).
 - Give values to inputs (temperature sources, $b$, and flow rate sources $f$).
 - Calculate steady-state response of the system of Diferential Algebraic Equations (DAE).
 - From the systems of Diferential Algebraic Equations (DAE), obtain the matrices $A_s$, $B_s$, $C_s$, and $D_s$ of the state-space representation.
 - Give the values of the input vector $u = [b_T^T, f_Q^T]^T$.
 - Obtain the steady-state response of the state-space representation.
 - Compare the results obtained for the system of Diferential Algebraic Equations (DAE) with the results obtained for the state-space representation. 
 - **Assignment 2**: Steady-state
     - [Grup 1, 2](https://classroom.github.com/a/6HWx5wze)
     - [Grup 3, 4](https://classroom.github.com/a/T6cSvhT4)
 
3. **Simulate step response**
 - Determine the time step and the settling time.
 - Give the input vector $u$.
 - Integrate in time the differential equations.
 - Plot the results.
 - Discuss the results.
 - **Assignment 3**: Simulate step response
     - [Grup 1, 2](https://classroom.github.com/a/1YlSy6uy)
     - [Grup 3, 4](https://classroom.github.com/a/XR32Fbwz)

4. **Simulate response to weather**
 - Define start and end time.
 - Prepare the inputs:
     - read weather data,
     - calculate the solar irradiance on the walls,
     - resample the weather data
     - give the other inputs (e.g., internal gains),
     - give the input vector in time.
 - Define the initial conditions.
 - Integrate in time.
 - Plot the results.
 - Discuss the results.
 - Implement other controllers (dead-band, model predictive control).
 - Discuss the results.
 - **Assignment 4**: Simulate response to weather
     - [Grup 1, 2](https://classroom.github.com/a/1VJkM4fh)
     - [Grup 3, 4](https://classroom.github.com/a/1VJkM4fh)
 
5. **Reproducible report**
 - Write the report in *Jupyter* notebooks.
 - Publish the report on *GitHub* and *MyBinder*.
 - **Assignment 5**: Reproducible report
     - [Grup 1, 2](https://classroom.github.com/a/4YDPKTYq)
     - [Grup 3, 4](https://classroom.github.com/a/Be3bPaux)
  
# Written report
The report will be written in *Jupyter* notebook, posted on *GitHub.com* and liked to *MyBinder.org*.

The general structure of the report:
- Front page: title, author(s), date.
- Contents.
- Description of the building: drawing, dimensions, materials, material properties, etc.
- Hypothesis: location, boundary conditions, schedule for usage, etc.
- Thermal model (with justifications).
- Mathematical model: Differential Algebraic Equations (matrices $A$, $G$, and $C$, vectors $b$ and $f$) and state-space representation (matrices $A$, $B$, $C$ and $D$ and vector $u$).
- Model implementation in Python.
- Steady-state results.
- Dynamic simulation results.
- Optimization (e.g., insulation, HVAC control, ventilation rate, solar shading).
