

- Video Toolbox
-  kVTPixelTransferPropertyKey_DestinationPixelAspectRatio 

Global Variable

# kVTPixelTransferPropertyKey_DestinationPixelAspectRatio

The pixel aspect ratio for destination image buffers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTPixelTransferPropertyKey_DestinationPixelAspectRatio: CFString
```

## Discussion

The value of this property is a doc://com.apple.documentation/documentation/corefoundation/cfdictionary-rum object with same keys as used in the kCVImageBufferPixelAspectRatioKey dictionary.

This property is ignored in kVTScalingMode_Normal. This property defaults to `NULL`, meaning 1:1 (for kVTScalingMode_CropSourceToCleanAperture) or no change in pixel aspect ratio (for kVTScalingMode_Letterbox and kVTScalingMode_Trim).

## See Also

### Configuration

let kVTPixelTransferPropertyKey_ScalingMode: CFString

Scaling mode for images during transfer between source and destination buffers.

Scaling Mode Constants

Supported constant values for the kVTPixelTransferPropertyKey_ScalingMode key.

let kVTPixelTransferPropertyKey_DestinationCleanAperture: CFString

The clean aperture for destination image buffers.

let kVTPixelTransferPropertyKey_DownsamplingMode: CFString

The specific chroma downsampling technique to be used.

Downsampling Mode Constants

Supported constant values for the kVTPixelTransferPropertyKey_DownsamplingMode key.

let kVTPixelTransferPropertyKey_DestinationColorPrimaries: CFString

The color primaries to be used for destination image buffers.

let kVTPixelTransferPropertyKey_DestinationTransferFunction: CFString

The color transfer function to be used for destination image buffers.

let kVTPixelTransferPropertyKey_DestinationICCProfile: CFString

The International Color Consortium (ICC) profile for destination image buffers.

let kVTPixelTransferPropertyKey_DestinationYCbCrMatrix: CFString

The color matrix to be used for YCbCr to RGB conversions involving the destination image buffers.

let kVTPixelTransferPropertyKey_RealTime: CFString

