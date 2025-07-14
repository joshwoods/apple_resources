

- QuickTime File Format
-  Video media information atom ('minf') 

Atom

# Video media information atom ('minf')

An atom that contains a number of other atoms that define specific characteristics of the video media data.

## Overview

Video media information atoms are the highest-level atoms in video media. These atoms contain a number of other atoms that define specific characteristics of the video media data.

The layout of a media information atom for video is as follows.

| Data | Type |
|----|----|
| Size | 4 bytes |
| Type = `'minf'` | 4 bytes |
| Video media information header atom | `'vmhd'`‡ |
| Handler reference atom | `'hdlr'`‡ |
| Data information atom | `'dinf'` |
| Sample table atom | `'stbl'` |

‡ denotes required atom.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this video media information atom.

Type

A 32-bit integer that identifies the atom type.

Video media information header atom

An atom that defines specific color and graphics mode information.

Handler reference atom

An atom that specifies the media handler component that is to be used to interpret the media’s data.

Data information atom

An atom that specifies the data handler component that provides access to the media data.

Sample table atom

An atom that contains information for converting from media time to sample number to sample location.

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

