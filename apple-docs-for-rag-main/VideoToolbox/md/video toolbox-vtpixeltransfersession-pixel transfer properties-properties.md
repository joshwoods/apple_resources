

- Video Toolbox
- VTPixelTransferSession
-  Pixel Transfer Properties 

API Collection

# Pixel Transfer Properties

Properties used to configure a VideoToolbox pixel transfer session.

## Topics

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

let kVTPixelTransferPropertyKey_DestinationYCbCrMatrix: CFString

The color matrix to be used for YCbCr to RGB conversions involving the destination image buffers.

let kVTPixelTransferPropertyKey_RealTime: CFString

