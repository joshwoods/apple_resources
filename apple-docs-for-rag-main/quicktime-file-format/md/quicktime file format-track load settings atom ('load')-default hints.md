

- QuickTime File Format
- Track load settings atom ('load')
-  Default hints 

Data field

# Default hints

A 32-bit integer containing playback hints.

## Overview

More than one flag may be enabled. Flags are enabled by setting them to `1`. The following flags are defined.

Double buffer  
This flag indicates playing the track using double-buffered I/O. This flag’s value is `0x0020`.

High quality  
This flag indicates displaying the track at the highest possible quality, without regard to real-time performance considerations. This flag’s value is `0x0100`.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this track load settings atom.

Type

A 32-bit integer that identifies the atom type.

Preload start time

A 32-bit integer specifying the starting time, in the movie’s time coordinate system, of a segment of the track that is to be preloaded.

Preload duration

A 32-bit integer specifying the duration, in the movie’s time coordinate system, of a segment of the track that is to be preloaded.

Preload flags

A 32-bit integer containing flags governing the preload operation.

