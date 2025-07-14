

- QuickTime File Format
- Font table atom ('ftab')
-  Font identifier 

Data field

# Font identifier

An unsigned 16-bit integer that identifies the font.

## Overview

This can be any number to uniquely identify this font in this table, but it must match the font number specified in the subtitle sample description and in any per-sample style records (`'styl'`).

## See Also

### Data fields

Size

An unsigned 32-bit integer holding the size of the font table atom.

Type

An unsigned 32-bit field.

Count

An unsigned 16-bit integer specifying how many fonts are described in this table.

Font name length

An unsigned 8-bit integer specifying the length of the font name in bytes.

Font name

Must be either “Serif” or “Sans-Serif”.

