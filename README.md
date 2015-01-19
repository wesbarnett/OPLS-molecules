# OPLS-molecules

These are some pdb and rtp files used in creating molecular topologies for use
in GROMACS. It's recommended that you first copy your GROMACS forcefield
directory before modifying anything and then setting the GMXLIB environmental
variable to the new location.

To create a molecular topology simply copy the relevant rtp file to your GMXLIB
directory's oplsaa.ff folder. Then run pdb2gmx on the corresponding pdb file.
For example, to create a methane topology copy "methane.rtp" to your GMXLIB
directory and then run:

````
pdb2gmx -f methane.pdb
````

Be sure to choose OPLS obviously.

I've tried to make sure that the output topologies are correct and don't have
anything missing. However, it is *your* job to ensure that they are correct and
there is no warranty that they are correct.
