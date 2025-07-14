

- QuickTime File Format
- Version check atom ('rmvc')
-  Check type 

Data field

# Check type

The type of check to perform, expressed as 16-bit integer.

## Overview

Set to `0` for a minimum version check, set to `1` for a required value after a binary `AND` of the Gestalt bitfield and the mask.

## See Also

### Data fields

Size

The number of bytes in this version check atom.

Type

The type of this atom.

Flags

A 32-bit integer.

Software package

A 32-bit Gestalt type specifying the software package to check for.

Version

An unsigned 32-bit integer containing either the minimum required version or the required value after a binary `AND` operation.

Mask

The mask for a binary `AND` operation on the Gestalt bitfield.

