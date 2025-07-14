

- QuickTime File Format
- Sample-to-group atom ('sbpd')
-  Table data 

Data field

# Table data

A table of sample count and group description index pairs.

## Mentioned in 

Representing encoder delay explicitly

## Overview

The layout of the table data is as follows:

| Data field              | Bytes |
|-------------------------|-------|
| Sample count            | 4     |
| Group description index | 4     |

Sample count  
A 32-bit integer that provides the number of consecutive media samples with the same sample group descriptor. The value is typically the same as in the sample size atom’s number of entries field.

Group description index  
A 32-bit integer the value of which is the index into the sample group description atom’s payload data table which describes the samples in this group. The index ranges from `1` to the number of payload data entries in the sample group description atom, or takes the value `0` to indicate that this group of samples is a member of no group of this type.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in this sample-to-group atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this sample-to-group atom.

Flags

A 3-byte reserved space.

Grouping type

A 32-bit integer identifying the grouping type.

Default length

A 32-bit integer indicating the length of the group entry in the payload data.

Entry count

A 32-bit integer giving the number of entries in the table data that follows.

