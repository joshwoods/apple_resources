

- QuickTime File Format
-  Track input map atom ('imap') 

Atom

# Track input map atom ('imap')

An atom that defines how data being sent to this track from its nonprimary sources is to be interpreted.

## Overview

This atom contains one or more track input atoms. Note that the track input map atom is a QT atom structure.

The layout of a track input map atom is as follows:

| Track input map atom | Bytes |
|----|----|
| Size | 4 |
| Type = `'imap'` | 4 |
| Track input atoms | Variable |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this track input map atom.

Type

A 32-bit integer that identifies the atom type.

Track input atoms

A list of track input atoms specifying how to use the input data.

## See Also

### Atoms for track input

Track input atom (' in')

An atom that specifies how to use the input data.

Input type atom (' ty')

An atom that specifies how to interpret track input data.

Object ID atom ('obid')

An atom that identifies an object, such as a sprite within a sprite track, in a track input atom.

