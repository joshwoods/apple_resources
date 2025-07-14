

- QuickTime File Format
-  Metadata atom ('meta') 

Atom

# Metadata atom ('meta')

An atom that is the container for carrying metadata.

## Overview

The following figure shows a sample layout of the metadata atom.

The metadata atom requires atoms with a solid outline, and atoms with a dotted outline are optional.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the atom.

Type

A 32-bit integer that identifies the atom type.

Metadata handler atom

An atom that defines the structure used for all types of metadata stored within the metadata atom.

Metadata header atom

An atom that holds the integer value for the next unique item identifier to assign.

Metadata item keys atom

An atom that holds a list of the metadata keys that may be present in the metadata atom.

Metadata item list atom

An atom that holds a list of actual metadata values that are present in the metadata atom.

Country list atom

An atom that lists items that are suitable for more than one country.

Language list atom

An atom that lists items that are suitable for more than one language.

## See Also

### Metadata structure

Metadata handler atom ('hdlr')

An atom that defines the structure used for all types of metadata stored within the metadata atom.

Metadata header atom ('mhdr')

An atom that holds the integer value for the next unique item identifier to assign.

