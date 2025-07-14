

- QuickTime File Format
-  Metadata locale atom ('loca') 

Atom

# Metadata locale atom ('loca')

An atom that tags a metadata value with a locale.

## Overview

A metadata value may optionally be tagged with its locale so that it may be chosen based upon the user’s language, country, and so on. This tagging makes it possible to include several keys of the same key type (e.g., copyright or scene description) but with differing locales for users with different languages or locations. The type of the metadata locale atom is `‘loca’`.

If the metadata locale atom is absent, metadata values should be considered appropriate for all locales.

The layout of a metadata locale atom is as follow:

| Data field | Bytes |
|----|----|
| Size | 4 |
| Type = `'loca'` | 4 |
| Locale string | variable |

## Topics

### Data fields

Size

A 32-bit unsigned integer that indicates the size in bytes of the atom structure.

Type

A 32-bit unsigned integer value.

Locale string

A string holding a language tag.

## See Also

### Describing timed metadata

Metadata key table atom ('keys')

An atom that contains a table of keys and mappings to payload data in the corresponding timed metadata media samples.

Bit rate atom ('btrt')

An atom that signals the bit rate information of a stream.

Metadata key atom

An atom that contains a key that corresponds to the timed metadata track containing it.

Metadata key declaration atom ('keyd')

An atom that holds the key namespace and key value of that namespace for the given values.

Metadata datatype definition atom ('dtyp')

An atom you use to specify the data type of the metadata key atom’s value.

