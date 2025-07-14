

- QuickTime File Format
-  Metadata handler atom ('hdlr') 

Atom

# Metadata handler atom ('hdlr')

An atom that defines the structure used for all types of metadata stored within the metadata atom.

## Mentioned in 

QuickTime File Format change log

## Overview

The metadata handler atom is a full atom with an atom type of `‘hdlr’`. It defines the structure used for all types of metadata stored within the metadata atom.

Note

A reader parsing a metadata atom should confirm the handler type in the metadata handler atom is ‘mdta’ before interpreting any other structures in the metadata atom according to the specification presented here. If the handler type is not ‘mdta’, the interpretation is defined by another specification.

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

Predefined

A 32-bit integer.

Handler type

A 32-bit integer that indicates the structure used in the metadata atom.

Reserved

An array of 3 const unsigned 32-bit integers.

Name

A string with a human-readable name for a metadata type.

## See Also

### Metadata structure

Metadata atom ('meta')

An atom that is the container for carrying metadata.

Metadata header atom ('mhdr')

An atom that holds the integer value for the next unique item identifier to assign.

