

- QuickTime File Format
- Media header atom ('mdhd')
-  Language 

Data field

# Language

A 16-bit integer that specifies the language code for this media.

## Overview

See Language code values for valid language codes. Also see Extended language tag atom ('elng') for the preferred code to use here if an extended language tag is also included in the media atom.

## See Also

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

Quality

A 16-bit integer that specifies the media’s playback quality.

