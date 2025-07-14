

- QuickTime File Format
- Media header atom ('mdhd')
-  Creation time 

Data field

# Creation time

A 32-bit integer that specifies the creation date for the media atom.

## Overview

Represent the calendar date and time in seconds since midnight, January 1, 1904, preferably using coordinated universal time (UTC).

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

