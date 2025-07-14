

- QuickTime File Format
-  Metadata key atom 

Atom

# Metadata key atom

An atom that contains a key that corresponds to the timed metadata track containing it.

## Mentioned in 

Constant-size timed metadata sample data

Timed metadata sample data format

## Overview

A metadata key atom is identified by a `local_key_id` corresponding to a 32-bit integer (or FourCC) type code local to the timed metadata track containing it. This `local_key_id` will correspond to atom types within the metadata sample data.

For example, if the metadata key atom has the atom type of `'stuf'`, any atoms of type `'stuf'` in timed metadata samples sharing this sample description hold the value for this key. Any value fitting in a 32-bit big endian integer can be used (such as `'stuf'` or the integer 72). If a FourCC is used, it is recommended that the value be mnemonic if possible. For example, a metadata key atom type of `‘actr’` might contain information about actors in a movie. See Timed metadata sample data format.

There are two reserved atom types for metadata key atoms: `0` and `0xFFFFFFFF`.

A `local_key_id` of `0` indicates the metadata key atom is unused and should not be interpreted. This indication allows the key to be marked as unused in the timed metadata sample description without requiring the sample description and parent atoms to be rewritten or resized.

A `local_key_id` of `0xFFFFFFFF` must not occur in a metadata key atom. It is reserved for future use and can occur as an atom type in timed metadata samples.

All other type codes are available for use as a `local_key_id`.

Note

Because the atoms within the metadata key table atom can take on any atom type, there should be no special interpretation of the type for contained atoms other than for the special value `0`. Therefore, including a `'free'` atom does not have the conventional meaning in the metadata key atom. It is recommended that writers avoid the use of overly confusing existing atom type codes.

Each metadata key atom contains a variable number of atoms that define the key structure, optionally the data type for values, and optionally locale information for values. Atoms may be introduced in the future.

A metadata key atom must contain a metadata declaration atom.

The layout of a metadata key atom is as follows:

| Data field | Bytes |
|----|----|
| Size | 4 |
| Type = `local_key_id` | 4 |
| Variable array of atoms | variable |

## Topics

### Data fields

Size

A 32-bit unsigned integer that indicates the size in bytes of the atom structure.

Type

A 32-bit unsigned integer value.

Variable array of atoms

An array of atoms carrying the definitions for key structure and other optional information.

## See Also

### Describing timed metadata

Metadata key table atom ('keys')

An atom that contains a table of keys and mappings to payload data in the corresponding timed metadata media samples.

Bit rate atom ('btrt')

An atom that signals the bit rate information of a stream.

Metadata key declaration atom ('keyd')

An atom that holds the key namespace and key value of that namespace for the given values.

Metadata datatype definition atom ('dtyp')

An atom you use to specify the data type of the metadata key atom’s value.

Metadata locale atom ('loca')

An atom that tags a metadata value with a locale.

