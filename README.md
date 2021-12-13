# Binary System with S-Type Planet
##### Brandon Shane, Arya Lakshmanan, Toshanraju Vysyaraju, and Ina Park

### Abstract
With the use of Newton's Law of Universal Gravitation, our team successfully modeled a binary system with an S-type orbit, and observed how the systems reacted under variations of different parameters. Although each variation produced drastically different scenarios, the model was successful through the observation that energy was conserved in each of the scenarios.

## Introduction
In a system where two stars and a planet are involved, there are two ways they can interact with each other. One is by a circumbinary orbit which is when the planet orbits both of the stars. The other is by an S-type orbit which occurs when the planet orbits just one of the stars. Using Newton’s Law of Universal Gravitation, our team modeled the 3-body problem of an S-type orbit, and analyzed how the systems would react under different variations of initial parameters. 

One of the ways we determined that our model was correct was due to the lack of deviations and the model’s predictable behavior (the orbits start and end at the same place) as seen in Figure 1.

## Results
We were able to successfully model the Three Body Problem and create S-Type binary system. We were able to successfully model two stars in a binary with a planet orbiting one of the stars. The resulting orbital paths can be seen in Figure 1. M1 and M2 have 1 and 2 solar masses respectively while M3 is 0.01 solar masses. Our simulation appears to have physical results. We can conclude this because while we set up Newtonian force equations and we solve those differential equations, we did not explicitly implement energy conservation into our code. Despite this, energy conservation is produced in our simulation implying that our results are physically meaningful. Energy conservation is explored in Figure 2. 

Our Three Body model is also sufficient to replicate other physical scenarios involving three objects at these masses. We explore changing initial conditions in `Variations`. We are able to create these additional models without needing to change the set up of differential equations. The only thing we need to vary to receive these different results is our initial conditions.

<p align="center">
    <img src="https://github.com/toshanv/S-Type-Binary/blob/master/images/variation1.gif" alt>
</p>
<p align="center">
    <em>Figure 1: Here the blue line represents the orbital path of our 1 solar mass star. The orange line represents the orbital path of our 2 solar mass. The green line represents the orbital path of our planet-like 0.01 $M_{\odot}$ object. Our S-type is nearly perfect with the orbit remaining stable for many periods. Our the planetary orbit also starts and ends at nearly the same point at the end of every period. As shown in Figure \ref{fig:engcons}, this model also accurately produces energy conservation which implies a connection to physical reality.</em>
</p>

<p align="center">
    <img src="https://github.com/toshanv/S-Type-Binary/blob/master/images/engcons.png" alt>
</p>
<p align="center">
    <em>Figure 2: In our simulation, we only solved differential equations of gravitational force. We did not explicitly work energy conservation into our work but it shows up nonetheless. This shows that we were successful in implementing our force equations and used them properly to generate our orbital paths. Since energy conservation is a natural result of our system, we can infer our results are accurate and meaningful.</em>
</p>

## Variations
### Variation 1 - Changing the planet's initial position to get the planet to transfer from M2 to M1
In this first variation, we increased the initial distance between M3 (the planet) and M2 (the star). The goal of this variation was to result in a simulation where M3 starts off by orbiting M2 and is eventually transferred over and begins to orbit M1. In order to do this, we increased the distance between M2 and M3 by 15.4\% and did not change any of the other initial conditions. This change of initial conditions results in M3 being less closely binded to M2. As a result, M3 starts off by orbiting M2 and is eventually transferred over to M1 and orbits M1 instead. This can be seen below:

<p align="center">
    <img src="https://github.com/toshanv/S-Type-Binary/blob/master/images/variation1.gif" alt>
</p>
<p align="center">
    <em>Figure 3: Changing the planet's initial position to get the planet to transfer from M2 to M1</em>
</p>

### Variation 2 - Changing the planet's initial position to get the planet to be slingshot out of the system
In this second variation, we severely increased the distance between M3 (the planet) and M2 (the star). The goal of this variation was to result in a simulation where M3 is slingshot out of the system. In order to do this, we severely increased the distance between M2 and M3. In the base model, M3 starts to the right of M2. In this model, we set M3 to start to the left of M2. We did this by decreasing the distance between M2 and M3 by 235\% and did not change any of the other initial conditions. This change of initial conditions results in M3 being slingshot out of the system after about 80 periods. This can be seen below:

<p align="center">
    <img src="https://github.com/toshanv/S-Type-Binary/blob/master/images/variation2.gif" alt>
</p>
<p align="center">
    <em>Variation 2 - Changing the planet's initial position to get the planet to be slingshot out of the system</em>
</p>

### Variation 3 - Creating highly eccentric orbits between M1 and M2
In this third variation, we created highly eccentric orbits between M1 and M2. In the base model, the eccentricity of the M1 and M2 orbit is 0.5 and the eccentricity of the M2 and M3 orbit is 0.3. The goal of this variation is to increase the eccentricity of the M1 and M2 orbit to get a highly eccentric orbit. In order to do this, we set the eccentricity of the M1 and M2 orbit to 0.8 and the eccentricity of the M2 and M3 orbit to 0.3 and did not change any of the other initial conditions. This change of initial conditions results in M3 being transferred back and forth between M2 and M1 (in the shown example, we only show M3 being transferred once as showing more than this results in an unclear plot with many overlapping lines). This can be seen below:

<p align="center">
    <img src="https://github.com/toshanv/S-Type-Binary/blob/master/images/variation3.gif" alt>
</p>
<p align="center">
    <em>Variation 3 - Creating highly eccentric orbits between M1 and M2</em>
</p>

### Variation 4 - 3D Model with perturbations in z-plane
In this fourth variation, we changed M3's velocity to be in the z direction and displayed a 3D plot. Our goal was to show a 3D Model of our simulation with perturbations in the z-plane. In order to do this, we changed the changed the direction of the velocity for M3 (the planet). In the base model, M3's velocity is in the y direction. However, in this first example of Variation 4, we set M3's velocity to be in the z direction without changing its magnitude and without changing any of the other initial conditions. This change of initial conditions results in the simulation below:

<p align="center">
    <img src="https://github.com/toshanv/S-Type-Binary/blob/master/images/variation4a-zplane.gif" alt>
</p>
<p align="center">
    <em>Variation 4a - 3D Model with perturbations in z-plane with M3's velocity in the z direction</em>
</p>

We also changed M3's initial motion's direction to be at 45&deg; between the y-axis and z-axis and plotted in a 3D plot. Changing only this and not changing any of the other initial conditions resulted in the simulation below:

<p align="center">
    <img src="https://github.com/toshanv/S-Type-Binary/blob/master/images/variation4b-yzplane.gif" alt>
</p>
<p align="center">
    <em>Variation 4b - 3D Model with perturbations in z-plane with M3's initial motion's direction to be at 45&deg; between the y-axis and z-axis</em>
</p>

### Variation 5 - Increasing M2 while keeping M1 and M3 constant
This fifth variation shows the scenario if M2 is much more massive than M1. We tripled M2 from 2 solar masses to 6 solar masses while keeping M1 and M3 constant (the same as the base model). M2's orbit is completely within M1's orbit. This makes sense in that as one of star masses continue to increase significantly compared to the other star, the model will look more and more like a 2-body model. Changing only M2 and not changing any of the other initial conditions resulted in the simulation below:

<p align="center">
    <img src="https://github.com/toshanv/S-Type-Binary/blob/master/images/variation5.gif" alt>
</p>
<p align="center">
    <em>Variation 5 - Increasing M2 while keeping M1 and M3 constant</em>
</p>

## Conclusions
Overall, with the use of Newton's Law of Universal Gravitation, our team was able to successfully model a 3-body system with an S-type orbit. We verified that it was successful due to the result that energy was conserved in our initial, base model, and continued to be conserved through every variation. 

To further our research on this topic, it would be interesting to observe how this model would change if we were to add another body or even n-number of bodies to the system, and observe how the simulation would expand. 
