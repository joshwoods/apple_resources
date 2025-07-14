

- QuickTime File Format
- Color parameter atom ('colr')
-  Color parameter type 

Data field

# Color parameter type

A 32-bit field containing a four-character code for the color parameter type.

## Overview

The currently defined types are `'nclc'` for video, and `'prof'` for print. The color parameter type distinguishes between print and video mappings. If the color parameter type is `'prof'`, then this field is followed by an ICC profile. This is the color model used by Apple’s ColorSync. The contents of this type are not defined in this documentation. Contact Apple for more information on the `'prof'` type `'colr'` extension. If the color parameter type is `'nclc'` then this atom contains the following fields:

- Primaries index

- Transfer function index

- Matrix index

## See Also

### Data fields

Size

An unsigned 32-bit integer holding the size of the color parameter atom.

Type

An unsigned 32-bit field.

Primaries index

A 16-bit unsigned integer containing an index into a table specifying the CIE 1931 xy chromaticity coordinates of the white point and the red, green, and blue primaries.

Transfer function index

A 16-bit unsigned integer containing an index into a table specifying the nonlinear transfer function coefficients used to translate between RGB color space values and Y´CbCr values.

Matrix index

A 16-bit unsigned integer containing an index into a table specifying the transformation matrix coefficients used to translate between RGB color space values and Y´CbCr values.

