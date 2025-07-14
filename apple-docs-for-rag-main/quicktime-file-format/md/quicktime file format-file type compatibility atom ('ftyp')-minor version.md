

- QuickTime File Format
- File type compatibility atom ('ftyp')
-  Minor version 

Data field

# Minor version

A 32-bit field that indicates the file format specification version.

## Overview

For QuickTime movie files, this takes the form of four binary-coded decimal values, indicating the century, year, and month of the *QuickTime File Format Specification*, followed by a binary coded decimal zero. For example, for the June 2004 minor version, this field is set to the BCD values `20 04 06 00`.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the atom.

Type

A 32-bit unsigned integer that identifies the atom type, typically represented as a four-character code.

Major brand

A 32-bit unsigned integer that represents a file format code.

Compatible brands

A series of unsigned 32-bit integers listing compatible file formats.

