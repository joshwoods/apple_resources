

- QuickTime File Format
-  Movie atom ('moov') 

Atom

# Movie atom ('moov')

An atom that specifies the information that defines a movie.

## Overview

You use movie atoms to specify the information that defines a movie — that is, the information that allows your application to interpret the sample data that is stored elsewhere. The movie atom usually contains a movie header atom, which defines the time scale and duration information for the entire movie, as well as its display characteristics. Existing movies may contain a movie profile atom, which summarizes the main features of the movie, such as the necessary codecs and maximum bit rate. In addition, the movie atom contains a track atom for each track in the movie.

The movie atom has an atom type of `'moov'`. It contains other types of atoms, including at least one of three possible atoms—the movie header atom (`'mvhd'`), the compressed movie atom (`'cmov'`), or a reference movie atom (`'rmra'`). An uncompressed movie atom can contain both a movie header atom and a reference movie atom, but it must contain at least one of the two. It can also contain several other atoms, such as a clipping atom (`'clip'`), one or more track atoms (`'trak'`), a color table atom (`'ctab'`), and a user data atom (`'udta'`).

Compressed movie atoms and reference movie atoms are discussed separately. This section describes normal uncompressed movie atoms.

The layout of movie atom is as follows.

| Data | Type |
|----|----|
| Size | 4 bytes |
| Type = `'moov'` | 4 bytes |
| Profile atom | `'prfl'` |
| Movie header atom | `'mvhd'`‡ |
| Movie clipping atom | `'clip'` |
| One or more Track atoms | `'trak'` |
| User data atom | `'udta'` |
| Color table atom | `'ctab'` |
| Compressed movie atom | `'cmov'` |
| Reference movie atom | `'rmra'` |

‡ denotes required atom.

## Topics

### Data fields

Size

The number of bytes in this movie atom.

Type

The type of this movie atom.

Profile atom

An atom that summarizes the features and complexity of a movie.

Movie header atom

An atom that specifies the characteristics of an entire QuickTime movie.

Movie clipping atom

An atom that specifies the clipping regions for movies and for tracks.

Track atoms

One or more atoms that define a single track of a movie.

User data atom

An atom where you define and store data associated with a QuickTime object.

Color table atom

An atom that defines a list of preferred colors for displaying the movie on devices that support only 256 colors.

Compressed movie atom

An atom you use to reduce file size and startup latency by compressing movie resources.

Reference movie atom

A reference movie atom contains references to one or more movies.

## See Also

### Describing movies

Movie header atom ('mvhd')

An atom that specifies the characteristics of an entire QuickTime movie.

Color table atom ('ctab')

An atom that defines a list of preferred colors for displaying the movie on devices that support only 256 colors.

User data atoms

Atoms you use to define and store data associated with a QuickTime object.

Interleaving movie data

Interleave data in your movie for optimal playback.

