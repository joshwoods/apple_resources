

- QuickTime File Format
- Handler reference atom ('hdlr')
-  Component subtype 

Data field

# Component subtype

A four-character code that identifies the type of the media handler or data handler.

## Overview

For media handlers, this field defines the type of data — for example, `'vide'` for video data, `'soun'` for sound data or `‘subt’` for subtitles. See Media data atom types for information about defined media data types.

For data handlers, this field defines the data reference type; for example, a component subtype value of `'alis'` identifies a file alias.

## See Also

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

Component manufacturer

Reserved.

Component flags

Reserved.

Component flags mask

Reserved.

Component name

A counted string that specifies the name of the component — that is, the media handler used when this media was created.

