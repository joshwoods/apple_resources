

- QuickTime File Format
- Sample-to-chunk atom ('stsc')
-  Type 

Data field

# Type

A 32-bit integer that identifies the atom type.

## Overview

This field must be set to `'stsc'`.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this sample-to-chunk atom.

Version

A 1-byte specification of the version of this sample-to-chunk atom.

Flags

A 3-byte space for sample-to-chunk flags.

Number of entries

A 32-bit integer containing the count of entries in the sample-to-chunk table.

Sample-to-chunk table

A table that maps samples to chunks.

