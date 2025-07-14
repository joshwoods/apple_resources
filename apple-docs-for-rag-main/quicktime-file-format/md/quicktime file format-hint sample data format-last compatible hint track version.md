

- QuickTime File Format
- Hint sample data format
-  Last compatible hint track version 

Data field

# Last compatible hint track version

A 16-bit unsigned integer indicating the oldest hint track version with which this hint track is backward-compatible.

## Overview

If your application understands the hint track version specified by this field, it can work with this hint track.

## See Also

### Data fields

Size

A 32-bit integer specifying the size of this sample description in bytes.

Data format

A four-character code indicating the data format of the hint track samples.

Reserved

Six bytes.

Data reference index

A field that indirectly specifies where to find the hint track sample data.

Hint track version

A 16-bit unsigned integer indicating the version of the hint track specification.

Max packet size

A 32-bit integer indicating the packet size limit, in bytes, used when creating this hint track.

Additional data table

A table of variable length containing additional information.

