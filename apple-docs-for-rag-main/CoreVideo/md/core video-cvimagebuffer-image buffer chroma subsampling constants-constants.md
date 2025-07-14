

- Core Video
- CVImageBuffer
-  Image Buffer Chroma Subsampling Constants 

API Collection

# Image Buffer Chroma Subsampling Constants

Constants that indicate the original format of subsampled data in the image buffer before conversion to 422/2vuy format.

## Overview

Use the kCVImageBufferChromaSubsamplingKey key to attach one of these values to the image buffer.

Note

To use thse constants, ensure that the image buffer data was converted to 4:2:2 format using simple pixel replication.

## Topics

### Constants

let kCVImageBufferChromaSubsampling_420: CFString

A key that indicates the original chroma-subsampled data used 4:2:0 formatting.

let kCVImageBufferChromaSubsampling_422: CFString

A key that indicates the original chroma-subsampled data used 4:2:2 formatting.

let kCVImageBufferChromaSubsampling_411: CFString

A key that indicates the original chroma-subsampled data used 4:1:1 formatting.

## See Also

### Constants

Image Buffer Attachment Keys

Keys that describe the attachment types associated with image buffers.

Image Buffer Clean Aperture Keys

Keys that describe the clean aperture of an image buffer.

Image Buffer Pixel Aspect Ratio Keys

Keys that describe the pixel aspect ratio of an image buffer.

Image Buffer Display Dimensions Keys

Keys that describe the display dimensions of an image buffer.

Image Buffer Field Detail Constants

Constants that indicate the field order of interlaced video in an image buffer.

Image Buffer YCbCr Matrix Constants

Constants that indicate the type of conversion matrix Core Video uses when it converts image buffer data from the YCbCr color space to the RGB color space.

Image Buffer Color Primaries Constants

Constants that indicate the color primaries gamut for the image buffer.

Image Buffer Transfer Function Constants

Constants that indicate the transfer function for the image buffer.

Image Buffer Chroma Location Constants

Constants that indicate locations for chroma samples in the image buffer.

