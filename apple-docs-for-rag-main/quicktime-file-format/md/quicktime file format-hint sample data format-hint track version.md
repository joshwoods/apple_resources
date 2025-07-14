

- QuickTime File Format
- Hint sample data format
-  Hint track version 

Data field

# Hint track version

A 16-bit unsigned integer indicating the version of the hint track specification.

## Overview

This is currently set to `1`.

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

Last compatible hint track version

A 16-bit unsigned integer indicating the oldest hint track version with which this hint track is backward-compatible.

Max packet size

A 32-bit integer indicating the packet size limit, in bytes, used when creating this hint track.

Additional data table

A table of variable length containing additional information.

