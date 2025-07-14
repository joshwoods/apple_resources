

- QuickTime File Format
- Sample size atom ('stsz')
-  Sample size table 

Data field

# Sample size table

A table containing the sample size information.

## Overview

The sample size table contains an entry for every sample in the media’s data stream. Each table entry contains a size field. The size field contains the size, in bytes, of the sample in question. The table is indexed by sample number — the first entry corresponds to the first sample, the second entry is for the second sample, and so on.

An example of a sample size table is as follows.

| Sample size | Sample   |
|-------------|----------|
| Size        | Sample 1 |
| Size        | Sample 2 |
| Size        | Sample 3 |
| Size        | Sample 4 |
| Size        | Sample 5 |

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

Sample size

A 32-bit integer specifying the sample size.

Number of entries

A 32-bit integer containing the count of entries in the sample size table.

