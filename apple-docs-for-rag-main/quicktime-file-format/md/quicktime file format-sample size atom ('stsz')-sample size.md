

- QuickTime File Format
- Sample size atom ('stsz')
-  Sample size 

Data field

# Sample size

A 32-bit integer specifying the sample size.

## Overview

If all the samples are the same size, this field contains that size value. If this field is set to `0`, then the samples have different sizes, and those sizes are stored in the sample size table.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this sample size atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this sample size atom.

Flags

A 3-byte space for sample size flags.

Number of entries

A 32-bit integer containing the count of entries in the sample size table.

Sample size table

A table containing the sample size information.

