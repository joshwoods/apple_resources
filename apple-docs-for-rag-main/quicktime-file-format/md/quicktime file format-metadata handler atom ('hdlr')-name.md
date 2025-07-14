

- QuickTime File Format
- Metadata handler atom ('hdlr')
-  Name 

Data field

# Name

A string with a human-readable name for a metadata type.

## Overview

The name is a NULL-terminated string in UTF-8 characters which gives a human-readable name for a metadata type, for debugging and inspection purposes.

The string may be empty or a single byte containing `0`.

## See Also

### Data fields

Size

A 32-bit unsigned integer that indicates the size in bytes of the atom structure.

Type

A 32-bit unsigned integer value.

Version

One byte.

Flags

Three bytes.

Predefined

A 32-bit integer.

Handler type

A 32-bit integer that indicates the structure used in the metadata atom.

Reserved

An array of 3 const unsigned 32-bit integers.

