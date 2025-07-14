

- QuickTime File Format
- Color parameter atom ('colr')
-  Matrix index 

Data field

# Matrix index

A 16-bit unsigned integer containing an index into a table specifying the transformation matrix coefficients used to translate between RGB color space values and Y´CbCr values.

## Overview

The table of matrixes specifies the matrix used during the translation.

## See Also

### Data fields

Size

An unsigned 32-bit integer holding the size of the color parameter atom.

Type

An unsigned 32-bit field.

Color parameter type

A 32-bit field containing a four-character code for the color parameter type.

Primaries index

A 16-bit unsigned integer containing an index into a table specifying the CIE 1931 xy chromaticity coordinates of the white point and the red, green, and blue primaries.

Transfer function index

A 16-bit unsigned integer containing an index into a table specifying the nonlinear transfer function coefficients used to translate between RGB color space values and Y´CbCr values.

