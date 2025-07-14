

- QuickTime File Format
- File type compatibility atom ('ftyp')
-  Major brand 

Data field

# Major brand

A 32-bit unsigned integer that represents a file format code.

## Overview

A 32-bit unsigned integer that should be set to `'qt '` (note the two trailing ASCII space characters) for QuickTime movie files. If a file is compatible with multiple brands, all such brands are listed in the Compatible brands fields, and the Major brand identifies the preferred brand or best use.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the atom.

Type

A 32-bit unsigned integer that identifies the atom type, typically represented as a four-character code.

Minor version

A 32-bit field that indicates the file format specification version.

Compatible brands

A series of unsigned 32-bit integers listing compatible file formats.

