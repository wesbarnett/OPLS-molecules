# OPLS-molecules

These are some pdb and rtp files used in creating molecular topologies for use
in GROMACS. It's recommended that you first copy your GROMACS forcefield
directory before modifying anything and then setting the GMXLIB environmental
variable to the new location.

To create a molecular topology simply copy all of the rtp files to your GMXLIB's
oplsaa.ff folder. Then run pdb2gmx on the molecule in which you are interested.
For example, for methane run:

````
gmx pdb2gmx -f methane.pdb
````

Be sure to choose OPLS obviously.

I've tried to make sure that the output topologies are correct and don't have
anything missing. However, it is *your* job to ensure that they are correct and
there is no warranty that they are correct. Some of the pdb files depend upon
multiple rtp files, which is why it's a good idea to copy all of them over.
