

- QuickTime File Format
-  Bit rate atom ('btrt') 

Atom

# Bit rate atom ('btrt')

An atom that signals the bit rate information of a stream.

## Overview

The optional bit rate atom may be present at the end of any timed metadata sample description to signal the bit rate information of a stream. The bit rate information can be used for buffer configuration.

The layout of a bit rate atom is as follows:

| Data field | Bytes |
|----|----|
| Size | 4 |
| Type = `'btrt'` | 4 |
| Buffer size | 4 |
| Max bit rate | 4 |
| Average bit rate | 4 |

## Topics

### Data fields

Size

A 32-bit unsigned integer that indicates the size in bytes of the atom structure.

Type

A 32-bit unsigned integer value.

Buffer size

A 32-bit unsigned integer that indicates the suggested size of the associated data buffer.

Max bit rate

A 32-bit unsigned integer that indicates the maximum bit rate in bits/second of the associated media stream.

Average bit rate

A 32-bit unsigned integer that indicates the average bit rate in bits/second of the associated media stream.

## See Also

### Describing timed metadata

Metadata key table atom ('keys')

An atom that contains a table of keys and mappings to payload data in the corresponding timed metadata media samples.

Metadata key atom

An atom that contains a key that corresponds to the timed metadata track containing it.

Metadata key declaration atom ('keyd')

An atom that holds the key namespace and key value of that namespace for the given values.

Metadata datatype definition atom ('dtyp')

An atom you use to specify the data type of the metadata key atom’s value.

Metadata locale atom ('loca')

An atom that tags a metadata value with a locale.

