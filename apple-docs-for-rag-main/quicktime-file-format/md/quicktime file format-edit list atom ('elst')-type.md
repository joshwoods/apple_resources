

- QuickTime File Format
- Edit list atom ('elst')
-  Type 

Data field

# Type

A 32-bit integer that identifies the atom type.

## Mentioned in 

Representing encoder delay explicitly

## Overview

This field must be set to `'elst'`.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this edit list atom.

Version

A 1-byte specification of the version of this edit list atom.

Flags

Three bytes of space for flags.

Number of entries

A 32-bit integer that specifies the number of entries in the edit list atom.

Edit list table

An array of 32-bit values, grouped into entries containing 3 values each.

