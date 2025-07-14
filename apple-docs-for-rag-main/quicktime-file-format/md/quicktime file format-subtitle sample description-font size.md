

- QuickTime File Format
- Subtitle sample description
-  Font size 

Data field

# Font size

An 8-bit value for the font size, expressed in points.

## Overview

The value should always be `0.05` multiplied by the video track header height. For example, if the video track header is 720 points in height, this should be `36` (points). This size should be used in the default style record and in any per-sample style records. If a subtitle does not fit in the text box, the subtitle media handler may choose to shrink the font size so that the subtitle fits.

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

Foreground color

A 32-bit RGBA color that specifies the text’s color, 8 bits each for red, green, blue, and alpha (transparency).

Font table

An atom that identifies the font to use to display the text.

