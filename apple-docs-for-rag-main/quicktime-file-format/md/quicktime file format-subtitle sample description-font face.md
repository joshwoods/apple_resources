

- QuickTime File Format
- Subtitle sample description
-  Font face 

Data field

# Font face

An 8-bit integer that indicates the font’s style.

## Overview

Set this field to `0` for normal text. You can enable other style options by using one or more of the bit masks listed in the following table.

| Value    | Meaning   |
|----------|-----------|
| `0x0001` | Bold      |
| `0x0002` | Italic    |
| `0x0004` | Underline |

## See Also

### Data fields

Display flags

A 32-bit integer containing flags that describe how the subtitle text should be drawn.

Reserved

An 8-bit integer.

Reserved

An 8-bit integer.

Reserved

A 32-bit integer.

Default text box

A 64-bit rectangle that specifies an area to receive text (each 16 bits indicate top, left, bottom, and right, respectively) within the subtitle track.

Reserved

A 32-bit value.

Font identifier

A 16-bit value that must be set to the same font identifier as in the font table.

Font size

An 8-bit value for the font size, expressed in points.

Foreground color

A 32-bit RGBA color that specifies the text’s color, 8 bits each for red, green, blue, and alpha (transparency).

Font table

An atom that identifies the font to use to display the text.

