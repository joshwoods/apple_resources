

- QuickTime File Format
- Track atoms
-  Track input map atoms 

API Collection

# Track input map atoms

Atoms that define how data being sent to this track from its nonprimary sources is to be interpreted.

## Overview

Track input map atoms define how data being sent to this track from its nonprimary sources is to be interpreted. Track references of type `'ssrc'` define a track’s secondary data sources. These sources provide additional data that is to be used when processing the track. Track input map atoms have an atom type value of `'imap'`.

## Topics

### Atoms for track input

Track input map atom ('imap')

An atom that defines how data being sent to this track from its nonprimary sources is to be interpreted.

Track input atom (' in')

An atom that specifies how to use the input data.

Input type atom (' ty')

An atom that specifies how to interpret track input data.

Object ID atom ('obid')

An atom that identifies an object, such as a sprite within a sprite track, in a track input atom.

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

Track load settings atom ('load')

An atom that indicates how the track is to be used in its movie.

Track reference atoms

Atoms that defines relationships between tracks.

