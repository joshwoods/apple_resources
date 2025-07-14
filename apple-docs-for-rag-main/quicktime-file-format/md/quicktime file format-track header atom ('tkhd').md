

- QuickTime File Format
-  Track header atom ('tkhd') 

Atom

# Track header atom ('tkhd')

An atom that specifies the characteristics of a single track within a movie.

## Overview

The track header atom specifies the characteristics of a single track within a movie. A track header atom contains a size field that specifies the number of bytes and a type field that indicates the format of the data (defined by the atom type `'tkhd'`).

The layout of a track header atom is as follows.

| Data field | Bytes |
|----|----|
| Size | 4 |
| Type | 4 |
| Version | 1 |
| Flags | 3 |
| Creation time | 4 |
| Modification time | 4 |
| Track ID | 4 |
| Reserved | 4 |
| Duration | 4 |
| Reserved | 8 |
| Layer | 2 |
| Alternate group | 2 |
| Volume | 2 |
| Reserved | 2 |
| Matrix structure | 36 |
| Track width | 4 |
| Track height | 4 |

The track header atom contains the track characteristics for the track, including temporal, spatial, and volume information.

## Topics

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

Layer

A 16-bit integer that indicates this track’s spatial priority in its movie.

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

Track height

A 32-bit fixed-point number that indicates the height of this track in pixels.

## See Also

### Describing tracks

Track atom ('trak')

An atom that defines a single track of a movie.

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

