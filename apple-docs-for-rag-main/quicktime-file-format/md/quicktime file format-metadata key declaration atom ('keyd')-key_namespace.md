

- QuickTime File Format
- Metadata key declaration atom ('keyd')
-  Key_namespace 

Data field

# Key_namespace

A 32-bit identifier describing the domain and the structure of the key value.

## Overview

For example, this could indicate that `key_value` is a reverse-address style string (such as “com.apple.quicktime.ISO6709”), a binary four-character code (such as a `'cprt'` user data key), a Uniform Resource Identifier (URI), or other structures (such as native formats from other metadata standards). New key namespaces must be registered but because a reverse-address style string can often be used, using the reverse-address key namespace may be sufficient for most uses.

## See Also

### Data fields

Size

A 32-bit unsigned integer that indicates the size in bytes of the atom structure.

Type

A 32-bit unsigned integer value.

Key_value array

An array of unsigned 8-bit bytes holding the key’s value.

