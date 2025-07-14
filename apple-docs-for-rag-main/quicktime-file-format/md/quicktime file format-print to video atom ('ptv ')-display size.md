

- QuickTime File Format
- Print to video atom ('ptv ')
-  Display size 

Data field

# Display size

A 16-bit little-endian integer indicating the display size for the movie.

## Overview

- `0` indicates playing the movie at its normal size

- `1` indicates playing the movie at double size

- `2` indicates playing the movie at half size

- `3` indicates scaling the movie to fill the screen

- `4` indicates playing the movie at its current size (this value is normally used when the print to video atom is inserted transiently and the movie has been temporarily resized).

## See Also

### Data fields

Reserved

A 16-bit integer.

Reserved

A 16-bit integer.

Play on open

An 8-bit Boolean value that indicates whether the movie plays when opened.

