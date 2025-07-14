

- Core Video
- CVImageBuffer
-  Image Buffer Attachment Keys 

API Collection

# Image Buffer Attachment Keys

Keys that describe the attachment types associated with image buffers.

## Overview

An image buffer associates its attachment keys in a CFDictionary instance. To read and write these image buffer attachments, use the CVBufferCopyAttachment(_:_:_:) and CVBufferSetAttachment(_:_:_:_:) functions or other CVBuffer functions. See the CVBuffer topic group for additional information.

## Topics

### Constants

let kCVImageBufferCGColorSpaceKey: CFString

A key to the color space of the image buffer.

let kCVImageBufferCleanApertureKey: CFString

A key to the dictionary describing the clean aperture for the image buffer.

let kCVImageBufferPreferredCleanApertureKey: CFString

A key to the dictionary describing the preferred clean aperture for the image buffer.

let kCVImageBufferFieldCountKey: CFString

A key to the field count for the image buffer.

let kCVImageBufferFieldDetailKey: CFString

A key to the field detail for an image buffer that indicates the order of interlaced video data in the image buffer.

let kCVImageBufferPixelAspectRatioKey: CFString

A key to the dictionary describing the pixel aspect ratio for the image buffer.

let kCVImageBufferDisplayDimensionsKey: CFString

A key to the dictionary describing the display dimensions for the image buffer.

let kCVImageBufferGammaLevelKey: CFString

A key to the gamma level for the image buffer.

let kCVImageBufferICCProfileKey: CFString

A key to the ICC color profile for the image buffer.

let kCVImageBufferYCbCrMatrixKey: CFString

A key to the YCbCr to RGB color conversion matrix for the image buffer.

let kCVImageBufferColorPrimariesKey: CFString

A key to the color primaries gamut for the image buffer.

let kCVImageBufferTransferFunctionKey: CFString

A key to the transfer function for the image buffer.

let kCVImageBufferChromaLocationTopFieldKey: CFString

A key to the location of chroma top field information in the image buffer.

let kCVImageBufferChromaLocationBottomFieldKey: CFString

A key to the location of chroma bottom field information in the image buffer.

let kCVImageBufferChromaSubsamplingKey: CFString

A key to the original format of subsampled data in the image buffer.

let kCVImageBufferAlphaChannelIsOpaque: CFString

A key to indicate whether the alpha channel is fully opaque.

let kCVImageBufferContentLightLevelInfoKey: CFString

A key to the content light level information.

let kCVImageBufferMasteringDisplayColorVolumeKey: CFString

A key to the mastering display color volume.

## See Also

### Constants

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

Image Buffer Chroma Subsampling Constants

Constants that indicate the original format of subsampled data in the image buffer before conversion to 422/2vuy format.

