

- QuickTime File Format
-  Metadata item keys atom ('keys') 

Atom

# Metadata item keys atom ('keys')

An atom that holds a list of the metadata keys that may be present in the metadata atom.

## Overview

The metadata item keys atom holds a list of the metadata keys that may be present in the metadata atom. This list is indexed starting with `1`; `0` is a reserved index value. The metadata item keys atom is a full atom with an atom type of `‘keys’`.

Note that:

- Indexes into the metadata item keys atom are 1-based (`1…entry_count`).

- Zero (`0`) is reserved and never used as an index.

- The structure of `key_value` depends upon the key namespace.

The following figure shows a typical metadata item keys atom.

The following figure shows an example of a metadata item keys atom consisting of three keys: two from one key namespace and a third from another key namespace.

| `'keys'`          |
|-------------------|
| `entry_count = 3` |

|  | `key_size (uint32)` | `key_namespace (uint32)` | `key_value (uint8[])` |
|----|----|----|----|
| 1 | `38` | `'mdta'` | `com.apple.quicktime.copyright` |
| 2 | `35` | `'mdta'` | `com.apple.quicktime.author` |
| 3 | `12` | `'udta'` | `@cpy` |

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

A 32-bit integer indicating the number of key arrays to follow in this atom.

Key_size

A 32-bit integer indicating the size of the entire structure containing a key definition.

Key_namespace

A 32-bit integer defining a naming scheme used for metadata keys.

Key_value_Key_size-8

An array of 8-bit integers, each containing the actual name of the metadata key.

## See Also

### Atoms

Country list atom ('ctry')

An atom that lists items that are suitable for more than one country.

Language list atom ('lang')

An atom that lists items that are suitable for more than one language.

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

