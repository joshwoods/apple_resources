

- QuickTime File Format
-  Language list atom ('lang') 

Atom

# Language list atom ('lang')

An atom that lists items that are suitable for more than one language.

## Overview

When one or more items must be identified as being suitable for more than one language, each list of languages is stored in this otherwise optional atom. The language list atom is a full atom with an atom type of ‘lang’.

Each list starts with a 2-byte count of the number of items in the list, and then each ISO 639-2/T code, packed into two bytes, according to the ISO Language Code definition in the MP4 specification.

The atom consists of a count of the number of lists, expressed as a 32-bit integer, and then these lists, appended end-to-end.

Note that:

- Indexes into the Language List atom are 1-based.

- Zero (0) is reserved and never used as an index.

- Currently, there is a limit of 255 languages that may be recorded in a Language List atom.

The following table shows an example Language List atom consisting of two language lists with three and two languages, respectively.

| Field size | Field | Field contents | Comment |
|----|----|----|----|
| 32-bit | atom_size | 26 | Size of this language list atom in bytes. |
| 32-bit | atom_type | `'lang'` |  |
| 32-bit | entry_count | 2 | Number of language lists. |
| 16-bit | language_count | 3 | Number of languages in language list 1. |
| 16-bit | language | 5575 | Packed ISO code for ‘eng’ (English) |
| 16-bit | language | 6721 | Packed ISO code for ‘fra’ (French) |
| 16-bit | language | 4277 | Packed ISO code for ‘deu’ (German) |
| 16-bit | language_count | 2 | Number of languages in language list 2. |
| 16-bit | language | 19969 | Packed ISO code for ‘spa’ (Spanish) |
| 16-bit | language | 16882 | Packed ISO code for ‘por’ (Portuguese) |

## Topics

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

A 32-bit integer indicating the number of language arrays to follow in this atom.

Language_count

A 16-bit integer indicating the number of languages in the array.

Language_Language_count

An array of 16-bit integers, defined according to the ISO 639-2/T definition of language codes.

## See Also

### Atoms

Country list atom ('ctry')

An atom that lists items that are suitable for more than one country.

Metadata item keys atom ('keys')

An atom that holds a list of the metadata keys that may be present in the metadata atom.

Metadata item list atom ('ilst')

An atom that holds a list of actual metadata values that are present in the metadata atom.

Metadata item atom

An atom that holds a metadata value.

Value atom

An atom that expresses a metadata value.

Item information atom ('itif')

An atom that contains information about the item, including item-specific flags and item optional identifier.

Name atom ('name')

An atom you use to provide a name for a metadata item.

Data atom ('data')

An atom that contains the type and locale specific value of metadata.

