

- QuickTime File Format
-  Metadata key table atom ('keys') 

Atom

# Metadata key table atom ('keys')

An atom that contains a table of keys and mappings to payload data in the corresponding timed metadata media samples.

## Overview

The metadata key table atom contains a table of keys and mappings to payload data in the corresponding timed metadata media samples. The type of the metadata key table atom is set to `‘keys’`.

The metadata key table atom contains one or more instances of metadata key atoms, one for each configuration of a key that may occur in the sample units of the track. For example, if there are two keys, there will be two metadata key atoms in the metadata key table atom—one for each key.

If the metadata key table atom does not contain a key for which a client is searching, no timed metadata media samples associated with this sample description contain values with that key.

If the metadata key table atom does contain a particular key, this does not guarantee that timed metadata media samples containing a value for the key were written. So, clients finding a key in the metadata key table atom may still need to look through the track’s timed metadata media samples for values to determine if the track has the particular metadata.

Note

Having the ability for the metadata key table atom to contain keys that are not associated with any instances of timed metadata media samples allows a metadata sample description to be populated with keys that might be discovered (say during a capture process) and then samples to be written with a binding only for the keys found. If a key is never used, there’s no requirement that the timed metadata sample description be rewritten to exclude the key that isn’t needed.

If it is possible to remove unused entries and rewrite the metadata sample description efficiently, this is preferred.

If a timed metadata track includes a key in the metadata sample description but has values using the key in associated media samples, the metadata sample description can still be rewritten to eliminate the key from the metadata key table atom. While the metadata values remain in associated media samples, the data is no longer reachable because the key is now gone. Care should be exercised if the values should themselves be removed from the movie file. Although not a requirement, the remaining but now unreachable data can be removed by copying only referenced metadata values when copying media samples to a new track.

The layout of a metadata key table atom is as follows:

| Data field | Bytes |
|----|----|
| Size | 4 |
| Type = `'keys'` | 4 |
| Metadata key table | variable |

## Topics

### Data fields

Size

A 32-bit unsigned integer that indicates the size in bytes of the atom structure.

Type

A 32-bit unsigned integer value.

Metadata key table

An array of metadata key atoms.

## See Also

### Describing timed metadata

Bit rate atom ('btrt')

An atom that signals the bit rate information of a stream.

Metadata key atom

An atom that contains a key that corresponds to the timed metadata track containing it.

Metadata key declaration atom ('keyd')

An atom that holds the key namespace and key value of that namespace for the given values.

Metadata datatype definition atom ('dtyp')

An atom you use to specify the data type of the metadata key atom’s value.

Metadata locale atom ('loca')

An atom that tags a metadata value with a locale.

