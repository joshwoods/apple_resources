

- QuickTime File Format
- Track input atom (' in')
-  Atom ID 

Data field

# Atom ID

A 32-bit integer relating this track input atom to its secondary input.

## Overview

The value of this field corresponds to the index of the secondary input in the track reference atom. That is, the first secondary input corresponds to the track input atom with an atom ID value of `1`; the second to the track input atom with an atom ID of `2`, and so on.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this track input atom.

Type

A 32-bit integer that identifies the atom type.

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

