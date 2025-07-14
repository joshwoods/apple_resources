

- Video Toolbox
-  kVTPixelTransferPropertyKey_DestinationYCbCrMatrix 

Global Variable

# kVTPixelTransferPropertyKey_DestinationYCbCrMatrix

The color matrix to be used for YCbCr to RGB conversions involving the destination image buffers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTPixelTransferPropertyKey_DestinationYCbCrMatrix: CFString
```

## Discussion

Specifying this value may lead to performance degradation, as a color matching operation may need to be performed between the source and the destination.

See kCMFormatDescriptionExtension_YCbCrMatrix in `CMFormatDescription.h` for possible values.

## See Also

### Configuration

let kVTPixelTransferPropertyKey_ScalingMode: CFString

Scaling mode for images during transfer between source and destination buffers.

Scaling Mode Constants

Supported constant values for the kVTPixelTransferPropertyKey_ScalingMode key.

let kVTPixelTransferPropertyKey_DestinationCleanAperture: CFString

The clean aperture for destination image buffers.

let kVTPixelTransferPropertyKey_DestinationPixelAspectRatio: CFString

The pixel aspect ratio for destination image buffers.

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

let kVTPixelTransferPropertyKey_RealTime: CFString

