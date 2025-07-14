

- QuickTime File Format
-  Object ID atom ('obid') 

Atom

# Object ID atom ('obid')

An atom that identifies an object, such as a sprite within a sprite track, in a track input atom.

## Overview

If the input is operating on an object within the track (for example, a sprite within a sprite track), an object ID atom must be included in the track input atom to identify the object.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this object ID atom.

Type

A 32-bit integer that identifies the atom type.

Object ID

A 32-bit integer identifying the object.

## See Also

### Atoms for track input

Track input map atom ('imap')

An atom that defines how data being sent to this track from its nonprimary sources is to be interpreted.

Track input atom (' in')

An atom that specifies how to use the input data.

Input type atom (' ty')

An atom that specifies how to interpret track input data.

