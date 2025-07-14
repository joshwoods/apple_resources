

- QuickTime File Format
-  Color table atom ('ctab') 

Atom

# Color table atom ('ctab')

An atom that defines a list of preferred colors for displaying the movie on devices that support only 256 colors.

## Overview

Color table atoms define a list of preferred colors for displaying the movie on devices that support only 256 colors. The list may contain up to 256 colors. These optional atoms have a type value of `'ctab'`. The color table atom contains a Macintosh color table data structure.

The layout of a color table atom is as follows.

| Data field | Bytes |
|----|----|
| Size | 4 |
| Type | 4 |
| Color table seed | 4 |
| Color table flags | 2 |
| Color table size | 2 |
| Color array | Variable |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this color table atom.

Type

A 32-bit integer that identifies the atom type.

Color table seed

A 32-bit integer.

Color table flags

A 16-bit integer.

Color table size

A 16-bit integer that indicates the number of colors in the following color array.

Color array

An array of colors.

## See Also

### Describing movies

Movie atom ('moov')

An atom that specifies the information that defines a movie.

Movie header atom ('mvhd')

An atom that specifies the characteristics of an entire QuickTime movie.

User data atoms

Atoms you use to define and store data associated with a QuickTime object.

Interleaving movie data

Interleave data in your movie for optimal playback.

