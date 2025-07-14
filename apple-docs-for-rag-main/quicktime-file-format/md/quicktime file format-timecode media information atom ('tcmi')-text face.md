

- QuickTime File Format
- Timecode media information atom ('tcmi')
-  Text face 

Data field

# Text face

A 16-bit integer that indicates the font’s style.

## Overview

Set this field to `0` for normal text. You can enable other style options by using one or more of the bit masks listed in the following table.

| Value    | Meaning   |
|----------|-----------|
| `0x0001` | Bold      |
| `0x0002` | Italic    |
| `0x0004` | Underline |
| `0x0008` | Outline   |
| `0x0010` | Shadow    |
| `0x0020` | Condense  |
| `0x0040` | Extend    |

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this time code media information atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this timecode media information atom.

Flags

A 3-byte space for timecode media information flags.

Text font

A 16-bit integer that indicates the font to use.

Text size

A 16-bit integer that specifies the point size of the time code text.

Reserved

A 16-bit integer that is reserved for use by Apple.

Text color

A 48-bit RGB color value for the timecode text.

Background color

A 48-bit RGB background color for the timecode text.

Font name

A Pascal string specifying the name of the timecode text’s font.

