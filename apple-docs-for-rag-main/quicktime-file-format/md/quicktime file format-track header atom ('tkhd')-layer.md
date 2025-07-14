

- QuickTime File Format
- Track header atom ('tkhd')
-  Layer 

Data field

# Layer

A 16-bit integer that indicates this track’s spatial priority in its movie.

## Overview

The QuickTime Movie Toolbox uses this value to determine how tracks overlay one another. Tracks with lower layer values are displayed in front of tracks with higher layer values.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this track header atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this track header.

Flags

Three bytes that are reserved for the track header flags.

Creation time

A 32-bit integer that indicates the creation calendar date and time for the track header.

Modification time

A 32-bit integer that indicates the last change date for the track header.

Track ID

A 32-bit integer that uniquely identifies the track.

Reserved

A 32-bit integer that is reserved for use by Apple.

Duration

A time value that indicates the duration of this track, in the movie’s time coordinate system.

Reserved

An 8-byte value that is reserved for use by Apple.

Alternate group

A 16-bit integer that identifies a collection of movie tracks that contain alternate data for one another.

Volume

A 16-bit fixed-point value that indicates how loudly to play this track’s sound.

Reserved

A 16-bit integer that is reserved for use by Apple.

Matrix structure

The matrix structure associated with this track.

Track width

A 32-bit fixed-point number that specifies the width of this track in pixels.

