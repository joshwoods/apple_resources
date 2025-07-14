

- QuickTime File Format
-  Media atom ('mdia') 

Atom

# Media atom ('mdia')

An atom that describes and defines a track’s media type and sample data.

## Overview

The media atom has an atom type of `'mdia'`. It must contain a media header atom (`'mdhd'`), and it can contain a handler reference (`'hdlr'`) atom, media information (`'minf'`) atom, and user data (`'udta'`) atom.

Note

Do not confuse the media atom (`'mdia'`) with the media data atom (`'mdat'`). The media atom contains only references to media data; the media data atom contains the actual media samples.

The layout of a media atom is as follows.

| Data | Type |
|----|----|
| Size | 4 bytes |
| Type = `'mdia'` | 4 |
| Media header atom | `'mdhd'`‡ |
| Extended language tag atom | `'elng'` |
| Handler reference atom | `'hdlr'` |
| Media information atom | `'minf'` |
| User data atom | `'udta'` |

‡ denotes required atom.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this media atom.

Type

A 32-bit integer that identifies the atom type.

Media header atom

This atom contains the standard media information.

Extended language tag atom

This atom contains the extended language tag describing the media language.

Handler reference atom

This atom identifies the media handler component that is to be used to interpret the media data.

Media information atom

This atom contains data specific to the media type for use by the media handler component.

User data atom

An atom where you define and store data associated with a QuickTime object.

## See Also

### Describing media

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

Base media info atom ('gmin')

An atom that defines the media’s control information, including graphics mode and balance information.

Data information atom ('dinf')

An atom that specifies the data handler component that provides access to the media data.

Media data reference atom ('dref')

An atom that contains tabular data that instructs the data handler component how to access the media’s data.

