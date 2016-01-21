# Reproducing
Reproducing the results of the article: D. Siracusa et al, "Resource Allocation Policies in SDM Optical Networks", ONDM, 2015.

# Simulation Setup

## Queue model 

- The simulation uses a **Poisson process arrivals** and an **exponentian holding time**;
- The **average network load** is expressed as the fraction of in-use of the total; 
- The connectons are accepted on their their **shortest path**, but the K-Shortest Path (KSP) routing algorithm (with K=3) is used to compute two additional spare paths to be used if the resource allocation on the first one fails, due to lack of resources.

## Topology

The network used in simulation is the Spanish Backbone Network, as showed in the figure below. 

![topology]

[topology]: https://github.com/alaelson/reproducing1/blob/master/figures/spanish_backbone.jpg?raw=true "Spanish backbone network"

<center>**Spanish backbone network**</center>

## Optical Network Setup

- 384 12.5 GHz spectral slots per spatial dimention (i.e., a standard C-band fiber with 96 50 GHz WDM channels);
- 4 independently modulated signals per transmitter. For 100 Gbps carries modulated using DP-QPSK, it requires 32 GHZ of spectrum and more 9 GHz of guard-band on each side of each spectral super-channel;
- The requests can be 100, 200, 300 or 400 Gbps, uniformly distributed, that were entail spectral super channels of 4, 7, 10 and 12 slots and spatial super channels of 4, 8, 12, 16 slots.






