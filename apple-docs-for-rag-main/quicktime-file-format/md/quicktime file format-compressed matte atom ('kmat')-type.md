

- QuickTime File Format
- Compressed matte atom ('kmat')
-  Type 

Data field

# Type

A 32-bit integer that identifies the atom type.

## Overview

This field must be set to `'kmat'`.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this compressed matte atom.

Version

A 1-byte specification of the version of this compressed matte atom.

Flags

Three bytes of space for flags.

Matte image description structure

An image description structure associated with this matte data.

Matte data

The compressed matte data, which is of variable length.

