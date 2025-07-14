

- QuickTime File Format
- Hint sample data format
-  Data format 

Data field

# Data format

A four-character code indicating the data format of the hint track samples.

## Overview

Only `'rtp '` is currently defined. Note that the fourth character in `'rtp '` is an ASCII blank space (`0x20`). Do not attempt to packetize data whose format you do not recognize.

## See Also

### Data fields

Size

A 32-bit integer specifying the size of this sample description in bytes.

Reserved

Six bytes.

Data reference index

A field that indirectly specifies where to find the hint track sample data.

Hint track version

A 16-bit unsigned integer indicating the version of the hint track specification.

Last compatible hint track version

A 16-bit unsigned integer indicating the oldest hint track version with which this hint track is backward-compatible.

Max packet size

A 32-bit integer indicating the packet size limit, in bytes, used when creating this hint track.

Additional data table

A table of variable length containing additional information.

