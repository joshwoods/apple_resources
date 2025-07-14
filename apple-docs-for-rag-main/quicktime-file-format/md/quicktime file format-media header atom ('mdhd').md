

- QuickTime File Format
-  Media header atom ('mdhd') 

Atom

# Media header atom ('mdhd')

An atom that specifies the characteristics of a media, including time scale and duration.

## Overview

The media header atom specifies the characteristics of a media, including time scale and duration. The media header atom has an atom type of `'mdhd'`.

The layout of a media header atom is as follows.

| Media header atom | Bytes |
|----|----|
| Size | 4 |
| Type | 4 |
| Version | 1 |
| Flags | 3 |
| Creation time | 4 |
| Modification time | 4 |
| Time scale | 4 |
| Duration | 4 |
| Language | 2 |
| Quality | 2 |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this media header atom.

Type

A 32-bit integer that identifies the atom type.

Version

One byte that specifies the version of this header atom.

Flags

Three bytes of space for media header flags.

Creation time

A 32-bit integer that specifies the creation date for the media atom.

Modification time

A 32-bit integer that specifies the last modification date for the media atom.

Time scale

A time value that indicates the time scale for this media.

Duration

The duration of this media in units of its time scale.

Language

A 16-bit integer that specifies the language code for this media.

Quality

A 16-bit integer that specifies the media’s playback quality.

## See Also

### Describing media

Media atom ('mdia')

An atom that describes and defines a track’s media type and sample data.

Extended language tag atom ('elng')

An atom that represents media language information.

Handler reference atom ('hdlr')

An atom that specifies the media handler component that is to be used to interpret the media’s data.

Media information atoms

An atom that contains a number of other atoms that define specific characteristics of the video media data.

Video media information atom ('minf')

An atom that contains a number of other atoms that define specific characteristics of the video media data.

Video media information header atom ('vmhd')

An atom that defines specific color and graphics mode information.

Sound media information atom ('minf')

An atom that contains a number of other atoms that define specific characteristics of the sound media data.

Sound media information header atom ('smhd')

An atom that stores the sound media’s control information, such as balance.

Base media information atom ('minf')

An atom that stores the media information for media types such as timed metadata, text, MPEG, time code, and music.

Base media information header atom ('gmhd')

An atom that indicates that this media information atom pertains to a base media.

Base media info atom ('gmin')

An atom that defines the media’s control information, including graphics mode and balance information.

Data information atom ('dinf')

An atom that specifies the data handler component that provides access to the media data.

Media data reference atom ('dref')

An atom that contains tabular data that instructs the data handler component how to access the media’s data.

