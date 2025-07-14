

- QuickTime File Format
- Chunk offset atom ('stco')
-  Type 

Data field

# Type

A 32-bit integer that identifies the atom type.

## Overview

This field must be set to `'stco'`.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this chunk offset atom.

Version

A 1-byte specification of the version of this chunk offset atom.

Flags

A 3-byte space for chunk offset flags.

Number of entries

A 32-bit integer containing the count of entries in the chunk offset table.

Chunk offset table

A chunk offset table consisting of an array of offset values.

