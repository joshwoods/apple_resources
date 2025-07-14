

- QuickTime File Format
-  User data atom ('udta') 

Atom

# User data atom ('udta')

An atom where you define and store data associated with a QuickTime object.

## Overview

The layout of a user data atom is as follows.

| Data field | Bytes |
|----|----|
| Size | 4 |
| Type | 4 |
| User data list | Variable |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this user data atom.

Type

A 32-bit integer that identifies the atom type.

User data list

A series of user data atoms.

## See Also

### Atoms for user data

Track name atom ('tnam')

An atom that provides a name for a track.

Print to video atom ('ptv ')

An atom you use to play the movie in full-screen mode, with no window and no visible controller.

