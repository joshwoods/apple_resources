

- QuickTime File Format
-  Track atom ('trak') 

Atom

# Track atom ('trak')

An atom that defines a single track of a movie.

## Overview

Track atoms have an atom type value of `'trak'`. The track atom requires a track header atom (`'tkhd'`) and a media atom (`'mdia'`). Other child atoms are optional, and may include a track clipping atom (`'clip'`), a track matte atom (`'matt'`), an edit atom (`'edts'`), a track reference atom (`'tref'`), a track load settings atom (`'load'`), a track input map atom (`'imap'`), and a user data atom (`'udta'`).

Note

The track atom layout contains an optional track profile atom `‘prfl’`. Track profile atoms are deprecated in the current version of QuickTime but may be present in existing QuickTime files. The inclusion here documents existing content containing profile atoms, they should not be used for new development.

The layout of a track atom is as follows.

| Data | Type |
|----|----|
| Size | 4 bytes |
| Type | 4 bytes |
| Track profile atom | `'prfl'` |
| Track header atom | `'tkhd'` |
| Track aperture mode dimensions atom | `'tapt'` |
| Clipping atom | `'clip'` |
| Track matte atom | `'matt'` |
| Edit atom | `'edts'` |
| Track reference atom | `'tref'` |
| Track exclude from autoselection atom | `'txas'` |
| Track load settings atom | `'load'` |
| Track input map atom | `'imap'` |
| Media atom | `'mdia'` |
| User-defined data atom | `'udta'` |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this track atom.

Type

A 32-bit integer that identifies the atom type.

Track profile atom

A child atom of movie atoms or track atoms.

Track header atom

An atom that specifies the characteristics of a single track within a movie.

Track aperture mode dimensions atom

A container atom that stores information for video correction in the form of three required atoms.

Clipping atom

An atom that specifies the clipping regions for movies and for tracks.

Track matte atom

An atom you use to visually blend the track’s image when it is displayed.

Edit atom

An atom that defines the portions of the media that are to be used to build up a track for a movie.

Track reference atom

An atom that defines relationships between tracks.

Track exclude from autoselection atom

An atom that indicates not to automatically select this track.

Track load settings atom

An atom that indicates how the track is to be used in its movie.

Track input map atom

An atom that defines how data being sent to this track from its nonprimary sources is to be interpreted.

Media atom

An atom that describes and defines a track’s media type and sample data.

User-defined data atom

An atom you use to define and store data associated with a QuickTime object.

## See Also

### Describing tracks

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

Track input map atoms

Atoms that define how data being sent to this track from its nonprimary sources is to be interpreted.

