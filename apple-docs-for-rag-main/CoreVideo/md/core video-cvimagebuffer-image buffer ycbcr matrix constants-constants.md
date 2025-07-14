

- Core Video
- CVImageBuffer
-  Image Buffer YCbCr Matrix Constants 

API Collection

# Image Buffer YCbCr Matrix Constants

Constants that indicate the type of conversion matrix Core Video uses when it converts image buffer data from the YCbCr color space to the RGB color space.

## Overview

Use the kCVImageBufferYCbCrMatrixKey key to attach one of these values to the image buffer.

## Topics

### Constants

let kCVImageBufferYCbCrMatrix_ITU_R_2020: CFString

let kCVImageBufferYCbCrMatrix_P3_D65: CFStringDeprecated

let kCVImageBufferYCbCrMatrix_ITU_R_709_2: CFString

A key to the conversion matrix for HDTV digital television images, that follows the ITU R 709 standard.

let kCVImageBufferYCbCrMatrix_ITU_R_601_4: CFString

A key to the conversion matrix for standard digital television images, that follows the ITU R 601 standard.

let kCVImageBufferYCbCrMatrix_SMPTE_240M_1995: CFString

A key to the conversion matrix for 1920 x 1135 HDTV images, that follows the SMPTE 240M 1995 standard.

let kCVImageBufferYCbCrMatrix_DCI_P3: CFStringDeprecated

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

Image Buffer Color Primaries Constants

Constants that indicate the color primaries gamut for the image buffer.

Image Buffer Transfer Function Constants

Constants that indicate the transfer function for the image buffer.

Image Buffer Chroma Location Constants

Constants that indicate locations for chroma samples in the image buffer.

Image Buffer Chroma Subsampling Constants

Constants that indicate the original format of subsampled data in the image buffer before conversion to 422/2vuy format.

