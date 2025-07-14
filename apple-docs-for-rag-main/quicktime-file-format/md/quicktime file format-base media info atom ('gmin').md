

- QuickTime File Format
-  Base media info atom ('gmin') 

Atom

# Base media info atom ('gmin')

An atom that defines the media’s control information, including graphics mode and balance information.

## Overview

The base media info atom, contained in the base media information header atom (`'gmhd'`), defines the media’s control information, including graphics mode and balance information.

The layout of the base media info atom is as follows.

| Base media info atom | Bytes |
|----|----|
| Size | 4 |
| Type | 4 |
| Version | 1 |
| Flags | 3 |
| Graphics mode | 2 |
| Opcolor | 6 |
| Balance | 2 |
| Reserved | 2 |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this base media info atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this base media information header atom.

Flags

A 3-byte space for base media information flags.

Graphics mode

A 16-bit integer that specifies the transfer mode.

Opcolor

Three 16-bit values that specify the red, green, and blue colors for the transfer mode operation indicated in the graphics mode field.

Balance

A 16-bit integer that specifies the sound balance of this media.

Reserved

Reserved for use by Apple.

## See Also

### Describing media

Media atom ('mdia')

An atom that describes and defines a track’s media type and sample data.

Media header atom ('mdhd')

An atom that specifies the characteristics of a media, including time scale and duration.

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

Data information atom ('dinf')

An atom that specifies the data handler component that provides access to the media data.

Media data reference atom ('dref')

An atom that contains tabular data that instructs the data handler component how to access the media’s data.

