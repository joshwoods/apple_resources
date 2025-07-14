

- QuickTime File Format
-  Track exclude from autoselection atom ('txas') 

Atom

# Track exclude from autoselection atom ('txas')

An atom that indicates not to automatically select this track.

## Mentioned in 

QuickTime File Format change log

## Overview

Some alternate tracks contain something other than a direct translation (or untranslated written form) of the primary content. Commentary tracks are one example. Don’t automatically select these tracks. The presence of the Track Exclude From Autoselection atom in a track indicates not to automatically select this track.

Ensure that such tracks have user-readable names that help users to identify the purpose of the track. These names are stored in one or more track name (`'tnam'`) atoms, each translated into a different language, within a user data (`'udta'`) atom within the `'trak'` atom.

The type of the Track Exclude From Autoselection atom is `'txas'`. This atom, if used, must be somewhere after the `'tkhd'` atom.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the track exclude from autoselection atom.

Type

A 32-bit integer that identifies the atom type.

## See Also

### Describing tracks

Track atom ('trak')

An atom that defines a single track of a movie.

Track header atom ('tkhd')

An atom that specifies the characteristics of a single track within a movie.

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

Track input map atoms

Atoms that define how data being sent to this track from its nonprimary sources is to be interpreted.

