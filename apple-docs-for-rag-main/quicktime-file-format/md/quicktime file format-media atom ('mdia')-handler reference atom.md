

- QuickTime File Format
- Media atom ('mdia')
-  Handler reference atom 

Data field

# Handler reference atom

This atom identifies the media handler component that is to be used to interpret the media data.

## Overview

See Handler reference atom ('hdlr') for more information.

Note that the handler reference atom tells you the kind of media this media atom contains—for example, video or sound. The layout of the media information atom is specific to the media handler that is to interpret the media. Media information atoms discusses how data may be stored in a media, using the video media format defined by Apple as an example.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this media atom.

Type

A 32-bit integer that identifies the atom type.

Media header atom

This atom contains the standard media information.

Extended language tag atom

This atom contains the extended language tag describing the media language.

Media information atom

This atom contains data specific to the media type for use by the media handler component.

User data atom

An atom where you define and store data associated with a QuickTime object.

