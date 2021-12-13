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
    <img src="https://github.com/toshanv/S-Type-Binary/blob/master/images/variation1.gif" alt>
</p>
<p align="center">
    <em>Figure 1: Here the blue line represents the orbital path of our 1 solar mass star. The orange line represents the orbital path of our 2 solar mass. The green line represents the orbital path of our planet-like 0.01 $M_{\odot}$ object. Our S-type is nearly perfect with the orbit remaining stable for many periods. Our the planetary orbit also starts and ends at nearly the same point at the end of every period. As shown in Figure \ref{fig:engcons}, this model also accurately produces energy conservation which implies a connection to physical reality.</em>
</p>
