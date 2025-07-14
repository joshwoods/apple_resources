

- QuickTime File Format
-  Data information atom ('dinf') 

Atom

# Data information atom ('dinf')

An atom that specifies the data handler component that provides access to the media data.

## Overview

The handler reference atom (described in Handler Reference Atoms) contains information specifying the data handler component that provides access to the media data. The data handler component uses the data information atom to interpret the media’s data. Data information atoms have an atom type value of `'dinf'`.

## Topics

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this data information atom.

Type

A 32-bit integer that identifies the atom type.

Data reference atom

An atom that contains tabular data that instructs the data handler component how to access the media’s data.

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

Base media info atom ('gmin')

An atom that defines the media’s control information, including graphics mode and balance information.

Media data reference atom ('dref')

An atom that contains tabular data that instructs the data handler component how to access the media’s data.

