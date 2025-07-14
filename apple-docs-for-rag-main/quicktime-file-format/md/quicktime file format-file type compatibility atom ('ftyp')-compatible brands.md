

- QuickTime File Format
- File type compatibility atom ('ftyp')
-  Compatible brands 

Data field

# Compatible brands

A series of unsigned 32-bit integers listing compatible file formats.

## Overview

The major brand must appear in the list of compatible brands. One or more “placeholder” entries with value zero are permitted; such entries should be ignored.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the atom.

Type

A 32-bit unsigned integer that identifies the atom type, typically represented as a four-character code.

Major brand

A 32-bit unsigned integer that represents a file format code.

Minor version

A 32-bit field that indicates the file format specification version.

