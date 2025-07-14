

- QuickTime File Format
- Metadata key declaration atom ('keyd')
-  Key_value array 

Data field

# Key_value array

An array of unsigned 8-bit bytes holding the key’s value.

## Overview

The interpretation of this array is defined by the associated `key_namespace` field. See the QuickTime metadata keys table for examples.

## See Also

### Data fields

Size

A 32-bit unsigned integer that indicates the size in bytes of the atom structure.

Type

A 32-bit unsigned integer value.

Key_namespace

A 32-bit identifier describing the domain and the structure of the key value.

