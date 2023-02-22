

SimpleNetwork below-ground competition concept. 
  
This concept allows the formation of groups of root grafted trees. Within these groups trees can exchange water driven by the water potential gradient between connected trees.
The model consists of three 'sub-models'

- Group formation
- Initialization of the root graft formation process
- Calculation of below-ground resources


## Group formation
In this sub-model the formation of is groups of connected trees in managed. Based on tree variables (*partners*), a graph dictionary and a link list a generated.

## Initialization rgf process  
The formation of root grafts between a pair of trees will be initialized when the following conditions are met

- the root plates of trees overlap (i.e. distance between trees < sum of root radii)
- the contact probability (i.e. 1 - distance/r_root_ij) is smaller than a randomly generated number
- the trees are not already connected with one another
- the trees are currently not in the process of rgf with one another

## Below-ground resources

In this concept, three volume flows describe the water flow in the tree:

- *water_absorbed*  that is the water absorbed by the tree from the soil column
- *water_available*  that is the water available for tree growth and maintenance, which corresponds to water uptake in the SimpleBettina model
- *water_exchanged*  that is the water exchanged between connected trees

The volume flows are calculated utilizing the electronic-hydraulic analogy. This allows the application of the Kirchhoff's laws, resulting in a set of linear equations.

<br>

This concept returns a multiplier for water loss or gain. 
This class is the basis (parent) for further Network concepts such as NetworkFixedSalinity.


