

- QuickTime File Format
-  Track atoms 

API Collection

# Track atoms

Atoms that define a single track of a movie.

## Overview

Track atoms define a single track of a movie. A movie may consist of one or more tracks. Each track is independent of the other tracks in the movie and carries its own temporal and spatial information. Each track atom contains its associated media atom.

Tracks are used specifically for the following purposes:

- To contain media data references and descriptions (media tracks).

- To contain modifier tracks (tweens, and so forth).

- To contain packetization information for streaming protocols (hint tracks). Hint tracks may contain references to media sample data or copies of media sample data. For more information about hint tracks, refer to Hint media.

Note

A QuickTime movie cannot consist solely of hint tracks or modifier tracks; there must be at least one media track. Furthermore, media tracks cannot be deleted from a hinted movie, even if the hint tracks contain copies of the media sample data—in addition to the hint tracks, the entire unhinted movie must remain.

## Topics

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

Track input map atoms

Atoms that define how data being sent to this track from its nonprimary sources is to be interpreted.

## See Also

### Movies

Movie atoms

Atoms that act as a container for the information that describes a movie’s data.

Media atoms

Atoms that describe and define a track’s media type and sample data.

Sample atoms

Atoms that describe samples, which are single elements in a sequence of time-ordered data.

Structuring movie data and features

Build movies with compressed or reference data, and add features like effect descriptions and alternate subtitle tracks.

