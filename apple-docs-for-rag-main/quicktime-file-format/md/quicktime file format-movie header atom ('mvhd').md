

- QuickTime File Format
-  Movie header atom ('mvhd') 

Atom

# Movie header atom ('mvhd')

An atom that specifies the characteristics of an entire QuickTime movie.

## Overview

You use the movie header atom to specify the characteristics of an entire QuickTime movie. The data contained in this atom defines characteristics of the entire QuickTime movie, such as time scale and duration. It has an atom type value of `'mvhd'`.

The following table shows the layout of the movie header atom. The movie header atom is a leaf atom.

| Data field | Bytes |
|----|----|
| Size | 4 |
| Type | 4 |
| Version | 1 |
| Flags | 3 |
| Creation time | 4 |
| Modification time | 4 |
| Time scale | 4 |
| Duration | 4 |
| Preferred rate | 4 |
| Preferred volume | 2 |
| Matrix structure | 36 |
| Preview time | 4 |
| Preview duration | 4 |
| Poster time | 4 |
| Selection time | 4 |
| Selection duration | 4 |
| Current time | 4 |
| Next track ID | 4 |

Note

Set the creation and modification date with coordinated universal time (UTC). In prior versions of the QuickTime file format, this was not specified, and these fields were commonly set to local time for the time zone where the movie was created.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this movie header atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this movie header atom.

Flags

Three bytes of space for future movie header flags.

Creation time

A 32-bit integer that specifies the creation calendar date and time for the movie atom.

Modification time

A 32-bit integer that specifies the calendar date and time of the last change to the movie atom.

Time scale

A time value that indicates the time scale for this movie.

Duration

A time value that indicates the duration of the movie in time scale units.

Preferred rate

A 32-bit fixed-point number that specifies the rate at which to play this movie.

Preferred volume

A 16-bit fixed-point number that specifies how loud to play this movie’s sound.

Reserved

Ten bytes reserved for use by Apple.

Matrix structure

The matrix structure associated with this movie.

Preview time

The time value in the movie at which the preview begins.

Preview duration

The duration of the movie preview in movie time scale units.

Poster time

The time value of the time of the movie poster.

Selection time

The time value for the start time of the current selection.

Selection duration

The duration of the current selection in movie time scale units.

Current time

The time value for current time position within the movie.

Next track ID

A 32-bit integer that indicates a value to use for the track ID number of the next track added to this movie.

## See Also

### Describing movies

Movie atom ('moov')

An atom that specifies the information that defines a movie.

Color table atom ('ctab')

An atom that defines a list of preferred colors for displaying the movie on devices that support only 256 colors.

User data atoms

Atoms you use to define and store data associated with a QuickTime object.

Interleaving movie data

Interleave data in your movie for optimal playback.

