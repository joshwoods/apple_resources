

- QuickTime File Format
- Video sample description ('stsd')
-  Depth 

Data field

# Depth

A 16-bit integer that indicates the pixel depth of the compressed image.

## Overview

Values of 1, 2, 4, 8 ,16, 24, and 32 indicate the depth of color images. The value 32 should be used only if the image contains an alpha channel. Values of 34, 36, and 40 indicate 2-, 4-, and 8-bit grayscale, respectively, for grayscale images.

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

Revision level

A 16-bit integer.

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

