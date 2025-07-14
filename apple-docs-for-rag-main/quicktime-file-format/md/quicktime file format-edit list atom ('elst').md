

- QuickTime File Format
-  Edit list atom ('elst') 

Atom

# Edit list atom ('elst')

An atom that maps from a time in a movie to a time in a media, and ultimately to media data.

## Mentioned in 

Representing encoder delay explicitly

Historical solution for implicit encoder delay

## Overview

You use the edit list atom to map from a time in a movie to a time in a media, and ultimately to media data. This information is in the form of entries in an edit list table. Edit list atoms have an atom type value of `'elst'`.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this edit list atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this edit list atom.

Flags

Three bytes of space for flags.

Number of entries

A 32-bit integer that specifies the number of entries in the edit list atom.

Edit list table

An array of 32-bit values, grouped into entries containing 3 values each.

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

Playing with edit lists

Repeat a segment of a movie without copying media with edit lists.

Track load settings atom ('load')

An atom that indicates how the track is to be used in its movie.

Track reference atoms

Atoms that defines relationships between tracks.

Track input map atoms

Atoms that define how data being sent to this track from its nonprimary sources is to be interpreted.

