

- QuickTime File Format
- User data atom ('udta')
-  User data list 

Data field

# User data list

A series of user data atoms.

## Overview

A user data list that is formatted as a series of atoms. Each data element in the user data list contains size and type information along with its payload data. For historical reasons, the data list is optionally terminated by a 32-bit integer set to `0`. If you are writing a program to read user data atoms, allow for the terminating `0`. However, if you are writing a program to create user data atoms, you can safely leave out the terminating `0`.

For a list of defined list entry types, see User data atoms.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this user data atom.

Type

A 32-bit integer that identifies the atom type.

