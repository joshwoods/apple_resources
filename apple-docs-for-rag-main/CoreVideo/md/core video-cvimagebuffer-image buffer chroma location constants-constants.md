

- Core Video
- CVImageBuffer
-  Image Buffer Chroma Location Constants 

API Collection

# Image Buffer Chroma Location Constants

Constants that indicate locations for chroma samples in the image buffer.

## Overview

For progressive-scan image data, use the kCVImageBufferChromaLocationTopFieldKey key to attach one of these values to the image buffer. For interlaced image data, attach values to the image buffer using the kCVImageBufferChromaLocationTopFieldKey and kCVImageBufferChromaLocationBottomFieldKey keys.

## Topics

### Constants

let kCVImageBufferChromaLocation_Left: CFString

A key that indicates the chroma sample is horizontally co-sited with the left column of luma samples, but centered vertically.

let kCVImageBufferChromaLocation_Center: CFString

A key that indicates the chroma sample is fully centered.

let kCVImageBufferChromaLocation_TopLeft: CFString

A key that indicates the chroma sample is co-sited with the top-left luma sample.

let kCVImageBufferChromaLocation_Top: CFString

A key that indicates the chroma sample is horizontally centered, but is co-sited with the top row of luma samples.

let kCVImageBufferChromaLocation_BottomLeft: CFString

A key that indicates the chroma sample is co-sited with the bottom-left luma sample.

let kCVImageBufferChromaLocation_Bottom: CFString

A key that indicates the chroma sample is horizontally centered, but is co-sited with the bottom row of luma samples.

let kCVImageBufferChromaLocation_DV420: CFString

A key that indicates the Cr and Cb samples are alternatingly co-sited with the left luma samples of the same field.

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

Image Buffer Chroma Subsampling Constants

Constants that indicate the original format of subsampled data in the image buffer before conversion to 422/2vuy format.

