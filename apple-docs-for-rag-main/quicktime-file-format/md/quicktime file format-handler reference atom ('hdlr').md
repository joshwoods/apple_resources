

- QuickTime File Format
-  Handler reference atom ('hdlr') 

Atom

# Handler reference atom ('hdlr')

An atom that specifies the media handler component that is to be used to interpret the media’s data.

## Overview

The handler reference atom has an atom type value of `'hdlr'`.

Historically, the handler reference atom was also used for data references. However, this isn’t the case anymore.

The handler atom within a media atom declares the process by which the media data in the stream may be presented, and thus, the nature of the media in a stream. For example, a video handler would handle a video track.

The layout of a handler reference atom is as follows.

| Handler reference atom | Bytes |
|----|----|
| Size | 4 |
| Type | 4 |
| Version | 1 |
| Flags | 3 |
| Component type | 4 |
| Component subtype | 4 |
| Component manufacturer | 4 |
| Component flags | 4 |
| Component flags mask | 4 |
| Component name | Variable |

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this handler reference atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this handler information.

Flags

A 3-byte space for handler information flags.

Component type

A four-character code that identifies the type of the handler.

Component subtype

A four-character code that identifies the type of the media handler or data handler.

Component manufacturer

Reserved.

Component flags

Reserved.

Component flags mask

Reserved.

Component name

A counted string that specifies the name of the component — that is, the media handler used when this media was created.

## See Also

### Describing media

Media atom ('mdia')

An atom that describes and defines a track’s media type and sample data.

Media header atom ('mdhd')

An atom that specifies the characteristics of a media, including time scale and duration.

Extended language tag atom ('elng')

An atom that represents media language information.

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

