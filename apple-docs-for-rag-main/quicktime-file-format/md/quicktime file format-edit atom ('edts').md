

- QuickTime File Format
-  Edit atom ('edts') 

Atom

# Edit atom ('edts')

An atom that defines the portions of the media that are to be used to build up a track for a movie.

## Overview

You use edit atoms to define the portions of the media that are to be used to build up a track for a movie. The edits themselves are contained in an edit list table, which consists of time offset and duration values for each segment. Edit atoms have an atom type value of `'edts'`.

In the absence of an edit list, the presentation of a track starts immediately. An empty edit is used to offset the start time of a track.

Note

If the edit atom or the edit list atom is missing, you can assume that the entire media is used by the track.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this edit atom.

Type

A 32-bit integer that identifies the atom type.

Edit list atom

An atom that maps from a time in a movie to a time in a media, and ultimately to media data.

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

Edit list atom ('elst')

An atom that maps from a time in a movie to a time in a media, and ultimately to media data.

Playing with edit lists

Repeat a segment of a movie without copying media with edit lists.

Track load settings atom ('load')

An atom that indicates how the track is to be used in its movie.

Track reference atoms

Atoms that defines relationships between tracks.

Track input map atoms

Atoms that define how data being sent to this track from its nonprimary sources is to be interpreted.

