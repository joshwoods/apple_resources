

- QuickTime File Format
-  Item information atom ('itif') 

Atom

# Item information atom ('itif')

An atom that contains information about the item, including item-specific flags and item optional identifier.

## Overview

The optional item information atom contains information about the item: item-specific flags and item optional identifier. This ID must be unique within the metadata atom. To simplify assignment of item identifiers, the metadata header atom’s nextItemInfo field can be used as described in Metadata header atom ('mhdr').

The item information atom must be present if the item has an assigned ID or has nonzero flags.

No flags are currently defined; they should be set to `0` in this version of the specification.

The item information atom is a full atom with an atom type of `‘itif’`.

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

Item_ID

An unsigned 32-bit integer, unique within the container.

## See Also

### Atoms

Country list atom ('ctry')

An atom that lists items that are suitable for more than one country.

Language list atom ('lang')

An atom that lists items that are suitable for more than one language.

Metadata item keys atom ('keys')

An atom that holds a list of the metadata keys that may be present in the metadata atom.

Metadata item list atom ('ilst')

An atom that holds a list of actual metadata values that are present in the metadata atom.

Metadata item atom

An atom that holds a metadata value.

Value atom

An atom that expresses a metadata value.

Name atom ('name')

An atom you use to provide a name for a metadata item.

Data atom ('data')

An atom that contains the type and locale specific value of metadata.

