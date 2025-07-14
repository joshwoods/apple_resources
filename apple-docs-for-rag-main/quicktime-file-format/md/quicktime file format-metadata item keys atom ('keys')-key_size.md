

- QuickTime File Format
- Metadata item keys atom ('keys')
-  Key_size 

Data field

# Key_size

A 32-bit integer indicating the size of the entire structure containing a key definition.

## Overview

The `key_size` = `sizeof(key_size) + sizeof(key_namespace) + sizeof(key_value)`. Since `key_size` and `key_namespace` are both 32 bit integers, together they have a size of 8 bytes. Hence, the `key_value` structure will be equal to `key_size - 8`.

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

Key_namespace

A 32-bit integer defining a naming scheme used for metadata keys.

Key_value_Key_size-8

An array of 8-bit integers, each containing the actual name of the metadata key.

