

- QuickTime File Format
- Track load settings atom ('load')
-  Preload duration 

Data field

# Preload duration

A 32-bit integer specifying the duration, in the movie’s time coordinate system, of a segment of the track that is to be preloaded.

## Overview

If the duration is set to –1, it means that the preload segment extends from the preload start time to the end of the track. All media data in the segment of the track defined by the preload start time and preload duration values should be loaded into memory when the movie is to be played.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this track load settings atom.

Type

A 32-bit integer that identifies the atom type.

Preload start time

A 32-bit integer specifying the starting time, in the movie’s time coordinate system, of a segment of the track that is to be preloaded.

Preload flags

A 32-bit integer containing flags governing the preload operation.

Default hints

A 32-bit integer containing playback hints.

