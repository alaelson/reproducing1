# Reproducing
Reproducing the results of the article: D. Siracusa et al, "Resource Allocation Policies in SDM Optical Networks", ONDM, 2015.

# Simulation Setup

## Queue model 

- The simulation uses a **Poisson process arrivals** and an **exponentian holding time**;
- The **average network load** is expressed as the fraction of in-use of the total; 
- The connectons are accepted on their their **shortest path**, but the K-Shortest Path (KSP) routing algorithm (with K=3) is used to compute two additional spare paths to be used if the resource allocation on the first one fails, due to lack of resources.

## Topology

![alt text](https://github.com/alaelson/reproducing1/blob/master/figures/spanish_backbone.jpg?raw=true "Spanish backbone network")