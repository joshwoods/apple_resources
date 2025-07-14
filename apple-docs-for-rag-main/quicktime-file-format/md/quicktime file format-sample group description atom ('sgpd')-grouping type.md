

- QuickTime File Format
- Sample group description atom ('sgpd')
-  Grouping type 

Data field

# Grouping type

A 32-bit integer that identifies the grouping type of this sample group description.

## Mentioned in 

Representing encoder delay explicitly

## Overview

Set to `‘roll’`.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this sample group description atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this sample group description.

Flags

A 3-byte reserved space.

Default length

A 32-bit integer indicating the length of the group entry in the payload data.

Entry count

A 32-bit integer giving the number of entries in the payload data field.

Payload data

A 16-bit signed integer giving the roll distance.

