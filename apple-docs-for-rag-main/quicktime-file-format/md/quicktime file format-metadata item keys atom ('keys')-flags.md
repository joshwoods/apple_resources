

- QuickTime File Format
- Metadata item keys atom ('keys')
-  Flags 

Data field

# Flags

Three bytes.

## Overview

Set to 0.

## See Also

### Data fields

Size

A 32-bit unsigned integer that indicates the size in bytes of the atom structure.

Type

A 32-bit unsigned integer value.

Version

One byte.

Entry_count

A 32-bit integer indicating the number of key arrays to follow in this atom.

Key_size

A 32-bit integer indicating the size of the entire structure containing a key definition.

Key_namespace

A 32-bit integer defining a naming scheme used for metadata keys.

Key_value_Key_size-8

An array of 8-bit integers, each containing the actual name of the metadata key.

