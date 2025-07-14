

- Core Video
- CVImageBuffer
-  Image Buffer Clean Aperture Keys 

API Collection

# Image Buffer Clean Aperture Keys

Keys that describe the clean aperture of an image buffer.

## Overview

Define these key-value pairs in a CFDictionary instance and use the kCVImageBufferCleanApertureKey or kCVImageBufferPreferredCleanApertureKey key to attach it to the image buffer. An image’s clean aperture is a region of video that’s free from transition artifacts caused by the encoding of the signal. This is the region of video to display.

## Topics

### Constants

let kCVImageBufferCleanApertureWidthKey: CFString

A key to the clean aperture width of the image buffer.

let kCVImageBufferCleanApertureHeightKey: CFString

A key to the clean aperture height of the image buffer.

let kCVImageBufferCleanApertureHorizontalOffsetKey: CFString

A key to the clean aperture horizontal offset value from the center of the image buffer.

let kCVImageBufferCleanApertureVerticalOffsetKey: CFString

A key to the clean aperture vertical offset value from the center of the image buffer.

## See Also

### Constants

Image Buffer Attachment Keys

Keys that describe the attachment types associated with image buffers.

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

Image Buffer Chroma Subsampling Constants

Constants that indicate the original format of subsampled data in the image buffer before conversion to 422/2vuy format.

