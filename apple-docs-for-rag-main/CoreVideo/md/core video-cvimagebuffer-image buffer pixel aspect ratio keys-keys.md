

- Core Video
- CVImageBuffer
-  Image Buffer Pixel Aspect Ratio Keys 

API Collection

# Image Buffer Pixel Aspect Ratio Keys

Keys that describe the pixel aspect ratio of an image buffer.

## Overview

Define these key-value pairs in a CFDictionary instance and use the kCVImageBufferPixelAspectRatioKey key to attach it to the image buffer.

## Topics

### Constants

let kCVImageBufferPixelAspectRatioHorizontalSpacingKey: CFString

A key to the horizontal component of the image buffer aspect ratio.

let kCVImageBufferPixelAspectRatioVerticalSpacingKey: CFString

A key to the vertical component of the image buffer aspect ratio.

## See Also

### Constants

Image Buffer Attachment Keys

Keys that describe the attachment types associated with image buffers.

Image Buffer Clean Aperture Keys

Keys that describe the clean aperture of an image buffer.

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

Image Buffer Chroma Subsampling Constants

Constants that indicate the original format of subsampled data in the image buffer before conversion to 422/2vuy format.

