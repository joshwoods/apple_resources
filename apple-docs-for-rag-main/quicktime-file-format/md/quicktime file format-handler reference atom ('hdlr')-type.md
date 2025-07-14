

- QuickTime File Format
- Handler reference atom ('hdlr')
-  Type 

Data field

# Type

A 32-bit integer that identifies the atom type.

## Overview

This field must be set to `'hdlr'`.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this handler reference atom.

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

