

- QuickTime File Format
-  Free space atom ('free') 

Atom

# Free space atom ('free')

An atom that designates unused space in the movie data file.

## Overview

Both `free` and `skip` atoms designate unused space in the movie data file. These atoms consist of only an atom header (size and type fields), followed by the appropriate number of bytes of free space. When reading a QuickTime movie, your application may safely skip these atoms. When writing or updating a movie, you may reuse the space associated with these atom types.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the atom.

Type

A 32-bit integer that identifies the atom type.

Free space

Bytes of free space.

## See Also

### Setting free space

Skip atom ('skip')

An atom that designates unused space in the movie data file.

Wide atom ('wide')

An atom that designates reserved space in the movie data file.

