

- Core Video
- CVImageBuffer
-  Image Buffer Color Primaries Constants 

API Collection

# Image Buffer Color Primaries Constants

Constants that indicate the color primaries gamut for the image buffer.

## Overview

Use the kCVImageBufferColorPrimariesKey key to attach one of these values to the image buffer. The color primaries gamut describes the rendering intent of an image, for use in color matching operations, along with a transfer function (See Image Buffer Transfer Function Constants for more information.).

## Topics

### Constants

let kCVImageBufferColorPrimaries_ITU_R_709_2: CFString

A key to the color primaries gamut for HD video.

let kCVImageBufferColorPrimaries_EBU_3213: CFString

A key to the color primaries gamut for PAL video.

let kCVImageBufferColorPrimaries_SMPTE_C: CFString

A key to the color primaries gamut for standard-definition video.

let kCVImageBufferColorPrimaries_DCI_P3: CFString

let kCVImageBufferColorPrimaries_ITU_R_2020: CFString

let kCVImageBufferColorPrimaries_P3_D65: CFString

let kCVImageBufferColorPrimaries_P22: CFString

A key to the color primaries gamut for sRGB video.

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

Image Buffer Transfer Function Constants

Constants that indicate the transfer function for the image buffer.

Image Buffer Chroma Location Constants

Constants that indicate locations for chroma samples in the image buffer.

Image Buffer Chroma Subsampling Constants

Constants that indicate the original format of subsampled data in the image buffer before conversion to 422/2vuy format.

