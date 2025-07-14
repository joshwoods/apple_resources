

- QuickTime File Format
- Video sample description ('stsd')
-  Revision level 

Data field

# Revision level

A 16-bit integer.

## Overview

Set to 0.

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

A 16-bit integer indicating the version number of the compressed data.

Vendor

A 32-bit integer that specifies the developer of the compressor that generated the compressed data.

Temporal quality

A 32-bit integer that indicates the degree of temporal compression.

Spatial quality

A 32-bit integer that indicates the degree of spatial compression.

Width

A 16-bit integer that specifies the width of the source image in pixels.

Height

A 16-bit integer that specifies the height of the source image in pixels.

Horizontal resolution

A 32-bit fixed-point number containing the horizontal resolution of the image in pixels per inch.

Vertical resolution

A 32-bit fixed-point number containing the vertical resolution of the image in pixels per inch.

Data size

A 32-bit integer.

Frame count

A 16-bit integer that indicates how many frames of compressed data are stored in each sample.

Compressor name

A 32-byte Pascal string containing the name of the compressor that created the image, such as “jpeg”.

