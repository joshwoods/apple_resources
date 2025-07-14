

- QuickTime File Format
- Version check atom ('rmvc')
-  Type 

Data field

# Type

The type of this atom.

## Overview

This field must be set to `'rmvc'`.

## See Also

### Data fields

Size

The number of bytes in this version check atom.

Flags

A 32-bit integer.

Software package

A 32-bit Gestalt type specifying the software package to check for.

Version

An unsigned 32-bit integer containing either the minimum required version or the required value after a binary `AND` operation.

Mask

The mask for a binary `AND` operation on the Gestalt bitfield.

Check type

The type of check to perform, expressed as 16-bit integer.

