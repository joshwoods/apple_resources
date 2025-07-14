

- QuickTime File Format
- Metadata item keys atom ('keys')
-  Key_namespace 

Data field

# Key_namespace

A 32-bit integer defining a naming scheme used for metadata keys.

## Overview

Location metadata keys, for example, use the `‘mdta’` key namespace.

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

Entry_count

A 32-bit integer indicating the number of key arrays to follow in this atom.

Key_size

A 32-bit integer indicating the size of the entire structure containing a key definition.

Key_value_Key_size-8

An array of 8-bit integers, each containing the actual name of the metadata key.

