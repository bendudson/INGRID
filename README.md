# INGRID
Interactive Grid Generator for Tokamak Boundary Region

Must have numpy, matplotlib, scipy, f90nml, and any fortran compiler. Gfortran
was used in the developement of this code.  To compile the fortran
scripts, call the makefile by typing make into the terminal while in
the src directory. This will generate the wrappers so the python codes
can call the fortran modules.

To install f90nml run
pip install f90nml
in the terminal window. This is used to read and write fortran namelist files.

Running the code:

python
>>> import sys
>>> #-use the path to Ingrid installation:
>>> sys.path.insert(1, '/home/umansky1/Projects/INGRID/INGRID_31jul19/src/')
>>> import Ingrid
>>>Ingrid.prep_input()
>>> Ingrid.run()
