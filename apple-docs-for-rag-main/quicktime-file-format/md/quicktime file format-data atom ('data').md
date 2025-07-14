

- QuickTime File Format
-  Data atom ('data') 

Atom

# Data atom ('data')

An atom that contains the type and locale specific value of metadata.

## Overview

The Data atom has an atom type of `‘data’`, and contains four bytes each of type and locale indicators, as specified in Type indicator and Locale indicator, and then the actual value of the metadata, formatted as required by the type.

## Topics

### Data fields

Type indicator

Four bytes that indicate a type of data that QuickTime supports.

Locale indicator

A four-byte value that indicates a locale.

Value

An array of bytes containing the value of the metadata.

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

Item information atom ('itif')

An atom that contains information about the item, including item-specific flags and item optional identifier.

Name atom ('name')

An atom you use to provide a name for a metadata item.

