

NetworkBettina death and growth concept. 
This concept allows water exchange between root grafted trees.
The concept is based on the Bettina single tree model as described in the ODD (appendix of https://doi.org/10.1016/j.ecolmodel.2018.10.005). 

The concept only works with a Network below-ground concept.

Available growth information for output (<growth_output > ... </growth_output>):

- root_surface_resistance
- xylem_resistance
- ag_resources
- bg_resources
- growth
- available_resources
- psi_zero
- salinity - **NOTE if trees are grafted this output is not correct. Use network output psi_osmo instead!**

Available network information for output (<network_output > ... </network_output>):
  
- partner ... list with tree names of partners;  
- potential_partner ... list with tree names of potential partners;  
- rgf ... counter that describes root graft formation status;  
- water_available ... available water for growth and maintenance in litre per timestep;  
- water_absorbed ... water absorbed from the soil in litre per timestep;  
- water_exchanged ... water exchanged between connected trees in litre per timestep 
- variant ... variant for root graft formation
- psi_osmo ... osmotic potential
- groupID ... unique group ID indicating which trees belong to the same group
- node_degree ... node degree indicates how many partners a tree has


