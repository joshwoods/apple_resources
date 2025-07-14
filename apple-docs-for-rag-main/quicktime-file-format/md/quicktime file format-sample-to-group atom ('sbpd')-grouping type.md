

- QuickTime File Format
- Sample-to-group atom ('sbpd')
-  Grouping type 

Data field

# Grouping type

A 32-bit integer identifying the grouping type.

## Mentioned in 

Representing encoder delay explicitly

## Overview

Set to `‘roll’`.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this sample-to-group atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this sample-to-group atom.

Flags

A 3-byte reserved space.

Default length

A 32-bit integer indicating the length of the group entry in the payload data.

Entry count

A 32-bit integer giving the number of entries in the table data that follows.

Table data

A table of sample count and group description index pairs.

