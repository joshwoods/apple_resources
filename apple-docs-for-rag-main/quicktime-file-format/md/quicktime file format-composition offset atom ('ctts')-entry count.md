

- QuickTime File Format
- Composition offset atom ('ctts')
-  Entry count 

Data field

# Entry count

A 32-bit unsigned integer that specifies the number of sample numbers in the array that follows.

## Overview

Following the entry count is a composition-offset table. The layout of the composition-offset table is as follows.

| Field             | Bytes |
|-------------------|-------|
| sampleCount       | 4     |
| compositionOffset | 4     |

sampleCount  
A 32-bit unsigned integer that provides the number of consecutive samples with the calculated composition offset in the field.

compositionOffset  
A 32-bit signed integer indicating the value of the calculated compositionOffset.

## See Also

### Data fields

Size

A 32-bit integer that specifies the number of bytes in the composition offset atom.

Type

A 32-bit integer that identifies the atom type.

Version

A 1-byte specification of the version of this atom.

Flags

A 3-byte space reserved for offset flags.

