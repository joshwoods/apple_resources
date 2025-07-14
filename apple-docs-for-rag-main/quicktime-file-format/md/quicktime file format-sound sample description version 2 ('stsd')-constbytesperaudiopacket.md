

- QuickTime File Format
- Sound sample description version 2 ('stsd')
-  constBytesPerAudioPacket 

Data field

# constBytesPerAudioPacket

A 32-bit unsigned integer set to the number of bytes per packet only if this value is constant.

## Overview

For other cases set to `0`.

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

always3

A 16-bit integer field.

always16

A 16-bit integer field.

alwaysMinus2

A 16-bit integer field.

always0

A 16-bit integer field.

always65536

A 32-bit integer field.

sizeOfStructOnly

A 32-bit integer field providing the offset to sound sample description structure’s extensions.

numAudioChannels

A 32-bit integer field set to the number of audio channels.

always7F000000

A 32-bit integer field.

