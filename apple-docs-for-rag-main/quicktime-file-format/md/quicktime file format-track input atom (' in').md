

- QuickTime File Format
-  Track input atom (' in') 

Atom

# Track input atom (' in')

An atom that specifies how to use the input data.

## Overview

The track input atom may contain two other types of atoms: input type atoms and object ID atoms. The input type atom is required; it specifies how the data is to be interpreted.

The track input atom layout is as follows:

| Track input atom | Bytes |
|----|----|
| Size | 4 |
| Type = `' in'` | 4 |
| Atom ID | 4 |
| Reserved | 2 |
| Child count | 2 |
| Reserved | 4 |
| Input type atom‡ | 12 |
| Object ID atom | 12 |

‡ Required atom.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this track input atom.

Type

A 32-bit integer that identifies the atom type.

Atom ID

A 32-bit integer relating this track input atom to its secondary input.

Reserved

A 16-bit integer.

Child count

A 16-bit integer specifying the number of child atoms in this atom.

Reserved

A 32-bit integer.

Input type atom

An atom that specifies how to interpret track input data.

Object ID atom

An atom that identifies an object, such as a sprite within a sprite track, in a track input atom.

## See Also

### Atoms for track input

Track input map atom ('imap')

An atom that defines how data being sent to this track from its nonprimary sources is to be interpreted.

Input type atom (' ty')

An atom that specifies how to interpret track input data.

Object ID atom ('obid')

An atom that identifies an object, such as a sprite within a sprite track, in a track input atom.

