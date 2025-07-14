

- QuickTime File Format
-  Metadata item list atom ('ilst') 

Atom

# Metadata item list atom ('ilst')

An atom that holds a list of actual metadata values that are present in the metadata atom.

## Overview

The metadata item list atom holds a list of actual metadata values that are present in the metadata atom. The metadata items are formatted as a list of items. The metadata item list atom is of type `‘ilst’` and contains a number of metadata items, each of which is an atom.

The following figure shows a metadata list atom and the item/key connection.

## Topics

### Data fields

Type

A 32-bit integer that identifies the atom type.

Item list

A list of metadata values and related keys.

## See Also

### Atoms

Country list atom ('ctry')

An atom that lists items that are suitable for more than one country.

Language list atom ('lang')

An atom that lists items that are suitable for more than one language.

Metadata item keys atom ('keys')

An atom that holds a list of the metadata keys that may be present in the metadata atom.

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

