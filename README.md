# Molecular modelling scripts

I have been meaning to make a collection of molecular modelling scripts. They're all jumbled up in different repositories, directories, and machines. I think this will be the beginning of a sensible collection. These scripts are licensed under the [Gnu General Public License, version 3.0+](https://choosealicense.com/licenses/gpl-3.0/).

## Contents

### cube2xyz

Forked from [julenl](https://github.com/julenl/molecular_modeling_scripts), it takes gaussian cube data, like electron density, and given a plane will write out an data file in the format `x,y,z,measured_value`. Basic usage (available also by `cube2xyz-v0.1.py -h`) is as follows.

````
usage: cube2xyz-v0.1.py [-h] -f FILE_NAME [-o OUT_FILE] [-pr PRINT_RANGE]
[-x X_COORD] [-y Y_COORD] [-z Z_COORD] [-pl] [-A]
[-no]cube2xyz can convert Gaussian type Cube files into “x y z value” columns, or
project values on planes (slizes) or segments. Optionally, it can directly
produce the plot for a faster visualization.

optional arguments:
-h, –help show this help message and exit
-f FILE_NAME, –file_name FILE_NAME
Name of cube file
-o OUT_FILE, –out_file OUT_FILE
Name of the file to which print the output (otherwise
printed to Standard Output).
-pr PRINT_RANGE, –print_range PRINT_RANGE
Print the range of x,y or z values and exit.
-x X_COORD, –x_coord X_COORD
Show only the values of x at this point.
-y Y_COORD, –y_coord Y_COORD
Show only the values of y at this point.
-z Z_COORD, –z_coord Z_COORD
Show only the values of z at this point.
-pl, –plot Plot graph using Mathplotlib.
-A, –angstrom Convert all distances to Angstrom.
-no, –no_output Do not produce any outupt.

Example usage: cube2xyz -f out.spol.cube -o xyzspol.dat -x 3.1 -pl -A
````



