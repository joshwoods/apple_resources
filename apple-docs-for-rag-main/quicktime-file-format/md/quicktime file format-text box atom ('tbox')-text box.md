

- QuickTime File Format
- Text box atom ('tbox')
-  Text box 

Data field

# Text box

A 64-bit rectangle that specifies an area to receive text (each 16 bits indicate top, left, bottom, and right, respectively) within the subtitle track.

## Overview

This rectangle must fill the track width dimensions exactly. The top and bottom coordinates can vary because they are used to place and size the subtitle text vertically. The top is used to place the text; the height is determined by the bottom minus the top. Neither the top nor the bottom should be outside the subtitle track dimensions. See Subtitle track header size and placement.

## See Also

### Data fields

Size

An unsigned 32-bit integer holding the size of the subtitle style atom.

Type

An unsigned 32-bit field.

