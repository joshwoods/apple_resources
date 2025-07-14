

- QuickTime File Format
-  Metadata item atom 

Atom

# Metadata item atom

An atom that holds a metadata value.

## Overview

Each item in the metadata item list atom is identified by its key. The atom type for each metadata item atom should be set equal to the index of the key for the metadata within the item atom, taking this index from the metadata item keys atom. In addition, each metadata item atom contains a Value Atom, to hold the value of the metadata item.

## Topics

### Data fields

Item_info

An optional item information atom.

Name

An optional name atom.

Data value atom

An array of value atoms.

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

Value atom

An atom that expresses a metadata value.

Item information atom ('itif')

An atom that contains information about the item, including item-specific flags and item optional identifier.

Name atom ('name')

An atom you use to provide a name for a metadata item.

Data atom ('data')

An atom that contains the type and locale specific value of metadata.

