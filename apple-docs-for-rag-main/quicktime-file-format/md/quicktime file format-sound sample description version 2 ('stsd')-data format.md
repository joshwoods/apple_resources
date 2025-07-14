

- QuickTime File Format
- Sound sample description version 2 ('stsd')
-  Data format 

Data field

# Data format

A 32-bit integer indicating the format of the stored data.

## Overview

This depends on the media type, but is usually either the compression format or the media type.

## See Also

### Data fields

Sample description size

A 32-bit integer indicating the number of bytes in the sample description.

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

constBitsPerChannel

A 32-bit integer field which is set only if constant and only for uncompressed audio.

