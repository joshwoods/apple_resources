

- QuickTime File Format
- Sound sample description version 0 ('stsd')
-  Sample size 

Data field

# Sample size

A 16-bit integer that specifies the number of bits in each uncompressed sound sample.

## Overview

Allowable values are 8 or 16. Formats using more than 16 bits per sample set this field to 16 and use sound description version 1.

## See Also

### Data fields

Sample description size

A 32-bit integer indicating the number of bytes in the sample description.

Data format

A 32-bit integer indicating the format of the stored data.

Reserved

Six bytes.

Data reference index

A 16-bit integer that contains the index of the data reference to use to retrieve data associated with samples that use this sample description.

Version

A 16-bit integer that holds the sample description version.

Revision level

A 16-bit integer.

Vendor

A 32-bit integer.

Number of channels

A 16-bit integer that indicates the number of sound channels used by the sound sample.

Compression ID

A 16-bit integer.

Packet size

A 16-bit integer.

Sample rate

A 32-bit unsigned fixed-point number (16.16) that indicates the rate at which the sound samples were obtained.

