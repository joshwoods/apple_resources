

- QuickTime File Format
-  Track load settings atom ('load') 

Atom

# Track load settings atom ('load')

An atom that indicates how the track is to be used in its movie.

## Overview

Track load settings atoms contain information that indicates how the track is to be used in its movie. Applications that read QuickTime files can use this information to process the movie data more efficiently. Track load settings atoms have an atom type value of `'load'`.

The layout of a track load settings atom is as follows.

| Track load settings atom | Bytes |
|----|----|
| Size | 4 |
| Type | 4 |
| Preload start time | 4 |
| Preload duration | 4 |
| Preload flags | 4 |
| Default hints | 4 |

## Topics

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

Default hints

A 32-bit integer containing playback hints.

## See Also

### Describing tracks

Track atom ('trak')

An atom that defines a single track of a movie.

Track header atom ('tkhd')

An atom that specifies the characteristics of a single track within a movie.

Track exclude from autoselection atom ('txas')

An atom that indicates not to automatically select this track.

Track aperture mode dimension atoms

Atoms that store information for each of the track aperture presentation modes.

Clipping atom ('clip')

An atom that specifies the clipping regions for movies and for tracks.

Clipping region atom ('crgn')

An atom that specifies the clipping region.

Track matte atom ('matt')

An atom you use to visually blend the track’s image when it is displayed.

Compressed matte atom ('kmat')

An atom that specifies the image description structure and the matte data associated with a particular matte atom.

Edit atom ('edts')

An atom that defines the portions of the media that are to be used to build up a track for a movie.

Edit list atom ('elst')

An atom that maps from a time in a movie to a time in a media, and ultimately to media data.

Playing with edit lists

Repeat a segment of a movie without copying media with edit lists.

Track reference atoms

Atoms that defines relationships between tracks.

Track input map atoms

Atoms that define how data being sent to this track from its nonprimary sources is to be interpreted.

