

- QuickTime File Format
-  Metadata header atom ('mhdr') 

Atom

# Metadata header atom ('mhdr')

An atom that holds the integer value for the next unique item identifier to assign.

## Overview

The metadata format optionally assigns unique identifiers to metadata items for such purposes as defining stable identifiers for external references into the set of metadata items. This is accomplished by including an item information atom in added metadata item atoms contained by the metadata item list atom. Such unique identifiers must be guaranteed to be unique.

To make the assignment of unique item identifiers more efficient, the metadata atom may contain a metadata header atom holding the integer value for the next unique item identifier to assign stored in the `nextItemID` field. In general it holds a value one greater than the largest identifier used so far.

Important

The metadata header atom must exist if there are metadata item atoms containing an item information atom indicating the item’s unique ID.

Upon assigning the identifier to a metadata item, if the value of the `nextItemID` field is less than `0xFFFFFFFF`, it should be incremented to the next unused value. If the value of `nextItemID` is equal to `0xFFFFFFFF`, it should not be changed: in that case, a search for an unused item identifier value in the range from `0` to `0xFFFFFFFF` is needed for all additions.

The metadata header atom is a full atom with an atom type of `‘mhdr’`.

Note

If the last metadata item with an item information atom is removed and value of `nextItemID` is `0xFFFFFFFF`, an implementation may reset the metadata header atom’s `nextItemID` value to `0` so that new assignments are again efficient (that is, they do not require a search for unused identifiers).

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

nextItemID

A 32-bit unsigned integer indicating the value to use for the item ID of the next item created or assigned an item ID.

## See Also

### Metadata structure

Metadata atom ('meta')

An atom that is the container for carrying metadata.

Metadata handler atom ('hdlr')

An atom that defines the structure used for all types of metadata stored within the metadata atom.

