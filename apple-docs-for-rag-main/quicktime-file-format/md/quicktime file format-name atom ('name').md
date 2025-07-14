

- QuickTime File Format
-  Name atom ('name') 

Atom

# Name atom ('name')

An atom you use to provide a name for a metadata item.

## Overview

The Name atom is a full atom with an atom type of `‘name’`. This atom contains a metadata name formatted as a string of UTF-8 characters, to fill the atom. It is optional. If it is not present, the item is unnamed, and cannot be referred to by name. Names are not user visible; they provide a way to refer to metadata items. The maximum length of a name may be limited in specific environments.

No two metadata items may have the same name.

## Topics

### Data fields

Version

One byte.

Flags

Three bytes.

Name

An array of bytes, constituting a UTF-8 string, containing the name.

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

Data atom ('data')

An atom that contains the type and locale specific value of metadata.

