

- QuickTime File Format
-  Metadata key declaration atom ('keyd') 

Atom

# Metadata key declaration atom ('keyd')

An atom that holds the key namespace and key value of that namespace for the given values.

## Overview

The metadata key declaration atom holds the key namespace and key value of that namespace for the given values. The type of the metadata key declaration atom is `‘keyd’`.

The layout of a metadata key declaration atom is as follows:

| Data field | Bytes |
|----|----|
| Size | 4 |
| Type = `'keyd'` | 4 |
| Key_namespace | 4 |
| Key_value array | variable |

## Topics

### Data fields

Size

A 32-bit unsigned integer that indicates the size in bytes of the atom structure.

Type

A 32-bit unsigned integer value.

Key_namespace

A 32-bit identifier describing the domain and the structure of the key value.

Key_value array

An array of unsigned 8-bit bytes holding the key’s value.

## See Also

### Describing timed metadata

Metadata key table atom ('keys')

An atom that contains a table of keys and mappings to payload data in the corresponding timed metadata media samples.

Bit rate atom ('btrt')

An atom that signals the bit rate information of a stream.

Metadata key atom

An atom that contains a key that corresponds to the timed metadata track containing it.

Metadata datatype definition atom ('dtyp')

An atom you use to specify the data type of the metadata key atom’s value.

Metadata locale atom ('loca')

An atom that tags a metadata value with a locale.

