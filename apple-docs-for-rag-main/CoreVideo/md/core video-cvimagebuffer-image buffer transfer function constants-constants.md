

- Core Video
- CVImageBuffer
-  Image Buffer Transfer Function Constants 

API Collection

# Image Buffer Transfer Function Constants

Constants that indicate the transfer function for the image buffer.

## Overview

Use the kCVImageBufferTransferFunctionKey key to attach one of these values to the image buffer. The transfer function describes the tonality of an image for use in color matching operations, along with a color primaries gamut (See Image Buffer Color Primaries Constants for more information.). Most apps should specify the kCVImageBufferTransferFunction_ITU_R_709_2 transfer function.

## Topics

### Constants

let kCVImageBufferTransferFunction_ITU_R_709_2: CFString

A key to the transfer function for high-definition and standard-definition video.

let kCVImageBufferTransferFunction_SMPTE_240M_1995: CFString

A key to the transfer function for HDTV interim video.

let kCVImageBufferTransferFunction_UseGamma: CFString

A key to the transfer function that’s defined by the gamma level value of the image buffer.

let kCVImageBufferTransferFunction_sRGB: CFString

let kCVImageBufferTransferFunction_ITU_R_2020: CFString

let kCVImageBufferTransferFunction_SMPTE_ST_428_1: CFString

let kCVImageBufferTransferFunction_ITU_R_2100_HLG: CFString

let kCVImageBufferTransferFunction_SMPTE_ST_2084_PQ: CFString

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

Image Buffer Chroma Location Constants

Constants that indicate locations for chroma samples in the image buffer.

Image Buffer Chroma Subsampling Constants

Constants that indicate the original format of subsampled data in the image buffer before conversion to 422/2vuy format.

