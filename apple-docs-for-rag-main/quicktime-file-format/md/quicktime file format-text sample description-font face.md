

- QuickTime File Format
- Text sample description
-  Font face 

Data field

# Font face

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

Display flags

A 32-bit integer containing flags that describe how the text should be drawn.

Text justification

A 32-bit integer that indicates how the text should be aligned.

Background color

A 48-bit RGB color that specifies the text’s background color.

Default text box

A 64-bit rectangle that specifies an area to receive text (top, left, bottom, right).

Reserved

A 64-bit value.

Font number

A 16-bit value.

Reserved

An 8-bit value.

Reserved

A 16-bit value.

Foreground color

A 48-bit RGB color that specifies the text’s foreground color.

Text name

A Pascal string specifying the name of the font to use to display the text.

