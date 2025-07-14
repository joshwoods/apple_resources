

- QuickTime File Format
- Track load settings atom ('load')
-  Preload flags 

Data field

# Preload flags

A 32-bit integer containing flags governing the preload operation.

## Overview

Only two flags are defined, and they are mutually exclusive. If this flag is set to `1`, the track is to be preloaded regardless of whether it is enabled. If this flag is set to `2`, the track is to be preloaded only if it is enabled.

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

Default hints

A 32-bit integer containing playback hints.

