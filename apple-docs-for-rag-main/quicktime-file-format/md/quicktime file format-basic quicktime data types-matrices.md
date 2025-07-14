

- QuickTime File Format
- Basic QuickTime data types
-  Matrices 

Article

# Matrices

QuickTime files use matrices to describe spatial information about many objects, such as tracks within a movie.

## Overview

A transformation matrix defines how to map points from one coordinate space into another coordinate space. By modifying the contents of a transformation matrix, you can perform several standard graphics display operations, including translation, rotation, and scaling. The matrix used to accomplish two-dimensional transformations is described mathematically by a 3-by-3 matrix.

All values in the matrix are 32-bit fixed-point numbers divided as `16.16`, except for the `{u, v, w}` column, which contains 32-bit fixed-point numbers divided as `2.30`. The following figure illustrates the matrix formula QuickTime uses to transform displayed objects.

When you specify a matrix in a movie header atom for a movie atom, QuickTime applies the transformation from the matrix to the atoms included in the movie atom, such as a clipping atom, one or more track atoms, a user data atom, and a color table atom.

## See Also

### Graphics and colors

Graphics modes

QuickTime files use graphics modes to describe how one video or graphics layer should be combined with the layers beneath it.

RGB colors

Colors stored as three consecutive unsigned 16-bit integers in the following order: red, green, blue.

Balance

Represent balance values with 16-bit fixed-point numbers.

