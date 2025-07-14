

- QuickTime File Format
- Subtitle sample description
-  Foreground color 

Data field

# Foreground color

A 32-bit RGBA color that specifies the text’s color, 8 bits each for red, green, blue, and alpha (transparency).

## Overview

For example, this would be `(0,0,0,255)` for opaque black or `(255,255,255,255)` for opaque white. Dark colors are not recommended, as the text could be placed onto a dark background.

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

Font face

An 8-bit integer that indicates the font’s style.

Font size

An 8-bit value for the font size, expressed in points.

Font table

An atom that identifies the font to use to display the text.

