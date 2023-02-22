
`Memory` is a mortality concept.

In `Memory`, a tree remembers its relative growth of the preceding N years (in m³ per memory period). 
Relative growth is defined as the fraction of growth in tree biomass (in m³ per m³).
If the relative growth falls below a certain threshold, a tree dies.  

The default threshold is 0.5 % (i.e. `<threshold> 0.005 </threshold>`).  
The default memory period is 1 year (i.e. `<period> 31557600 </period>`).

This concept is based on mechanistic causes, e.g. slowing down of growth due external perturbations. 
A tree can survive a period of resource scarcity but if conditions do not improve, the tree dies.  
No tree dies of random reasons.
