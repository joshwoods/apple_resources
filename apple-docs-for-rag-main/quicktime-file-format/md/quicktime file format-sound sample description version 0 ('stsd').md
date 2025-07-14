

- QuickTime File Format
-  Sound sample description version 0 ('stsd') 

Atom

# Sound sample description version 0 ('stsd')

A sound sample description that supports only uncompressed audio in raw or twos-complement format.

## Overview

There are currently three versions of the sound sample description, versions 0, 1 and 2. Version 0 supports only uncompressed audio in raw (`'raw '`) or twos-complement (`'twos'`) format, although these are sometimes incorrectly specified as either `'NONE'` or `0x00000000`.

Version 0 of the sound description format assumes uncompressed audio in `'raw '` or `'twos'` format, 1 or 2 channels, 8 or 16 bits per sample, and a compression ID of `0`.

## Topics

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

Sample size

A 16-bit integer that specifies the number of bits in each uncompressed sound sample.

Compression ID

A 16-bit integer.

Packet size

A 16-bit integer.

Sample rate

A 32-bit unsigned fixed-point number (16.16) that indicates the rate at which the sound samples were obtained.

## See Also

### Using sample descriptions

Sound sample description version 1 ('stsd')

An extended sound sample description that supports compressed audio, and includes the ability to add atoms to the sound description.

Sound sample description version 2 ('stsd')

An updated sound sample description that adds high resolution audio.

