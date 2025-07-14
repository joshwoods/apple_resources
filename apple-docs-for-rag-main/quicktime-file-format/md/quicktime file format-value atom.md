

- QuickTime File Format
-  Value atom 

Atom

# Value atom

An atom that expresses a metadata value.

## Overview

The value of the metadata item is expressed as immediate data in a value atom. The value atom starts with two fields: a type indicator, and a locale indicator. Both the type and locale indicators are four bytes long. There may be multiple ‘value’ entries, using different type, country or language codes (see Data ordering for the required ordering).

## Topics

### Data fields

Type indicator

Four bytes that indicate a type of data that QuickTime supports.

Locale indicator

A four-byte value that indicates a locale.

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

Item information atom ('itif')

An atom that contains information about the item, including item-specific flags and item optional identifier.

Name atom ('name')

An atom you use to provide a name for a metadata item.

Data atom ('data')

An atom that contains the type and locale specific value of metadata.

