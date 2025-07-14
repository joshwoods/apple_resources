

- Video Toolbox
-  kVTPixelTransferPropertyKey_ScalingMode 

Global Variable

# kVTPixelTransferPropertyKey_ScalingMode

Scaling mode for images during transfer between source and destination buffers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTPixelTransferPropertyKey_ScalingMode: CFString
```

## Discussion

Depending on the scaling mode, scaling may take into account:

- The full image buffer width and height of the source and destination

- The clean aperture attachment (kCVImageBufferCleanApertureKey) on the source image buffer

- The pixel aspect ratio attachment (kCVImageBufferPixelAspectRatioKey) on the source image buffer

- The destination clean aperture (kVTPixelTransferPropertyKey_DestinationCleanAperture)

- The destination pixel aspect ratio (kVTPixelTransferPropertyKey_DestinationPixelAspectRatio)

The destination image buffer’s clean aperture and pixel aspect ratio attachments are not taken into account, and are overwritten.

## See Also

### Configuration

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

let kVTPixelTransferPropertyKey_DestinationYCbCrMatrix: CFString

The color matrix to be used for YCbCr to RGB conversions involving the destination image buffers.

let kVTPixelTransferPropertyKey_RealTime: CFString

