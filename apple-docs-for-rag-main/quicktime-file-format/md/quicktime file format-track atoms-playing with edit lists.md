

- QuickTime File Format
- Track atoms
-  Playing with edit lists 

Article

# Playing with edit lists

Repeat a segment of a movie without copying media with edit lists.

## Overview

A segment of a movie can be repeated without duplicating media data by using edit lists. Suppose you have a single-track movie whose media time scale is `100` and track duration is `1000` (10 seconds). For this example the movie’s time scale is `600`. If there are no edits in the movie, the edit atom would contain the data values:

```
Edit list atom
├── Atom size: 36
├── Atom type: 'edts'
└── Edit list table atom
    ├── Atom size: 28
    ├── Atom type: 'elst'
    ├── Version/Flags: 0
    ├── Number of entries: 2
    ├── Track duration: 6000 (10 seconds)
    ├── Media time: 0
    └── Media rate: 1.0
```

Because this is a single-track move, the track’s duration in the track header atom is `6000` and the movie’s duration in the movie header atom is `6000`.

If you change the track to play the media from time `0` to time `2` seconds, and then play the media from time `0` to time `10` seconds, the edit atom would now contain these data values:

```
Edit list atom
├── Atom size: 48
├── Atom type: 'edts'
└── Edit list table atom
    ├── Atom size: 40
    ├── Atom type: 'elst'
    ├── Version/Flags: 0
    ├── Number of entries: 2
    ├── Track duration[1]: 1200 (2 seconds)
    ├── Media time[1]: 0
    ├── Media rate[1]: 1.0
    ├── Track duration[2]: 6000 (10 seconds)
    ├── Media time[2]: 0
    └── Media rate[2]: 1.0
```

Because the track is now 2 seconds longer, the track’s duration in the track header atom must now be `7200`, and the movie’s duration in the movie header atom must also be `7200`.

Currently, the media plays from time `0` to time `2`, then plays from time `0` to time `10`. If you take that repeated segment at the beginning (time `0` to time `2`) and play it at double speed to maintain the original duration, the edit atom would now contain the following values:

```
Edit list atom
├── Atom size: 60
├── Atom type: 'edts'
└── Edit list table atom
    ├── Atom size: 52
    ├── Atom type: 'elst'
    ├── Version/Flags: 0
    ├── Number of entries: 3
    ├── Track duration[1]: 600 (1 second)
    ├── Media time[1]: 0
    ├── Media rate[1]: 2.0
    ├── Track duration[2]: 600 (1 second)
    ├── Media time[2]: 0
    ├── Media rate[2]: 2.0
    ├── Track duration[3]: 4800 (8 seconds)
    ├── Media time[3]: 200
    └── Media rate[3]: 1.0
```

Because the track is now back to its original duration of 10 seconds, its duration in the track header atom is `6000`, and the movie’s duration in the movie header atom is `6000`.

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

Track load settings atom ('load')

An atom that indicates how the track is to be used in its movie.

Track reference atoms

Atoms that defines relationships between tracks.

Track input map atoms

Atoms that define how data being sent to this track from its nonprimary sources is to be interpreted.

