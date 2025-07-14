

- Video Toolbox
- VTPixelTransferSession
- Pixel Transfer Properties
-  Scaling Mode Constants 

API Collection

# Scaling Mode Constants

Supported constant values for the kVTPixelTransferPropertyKey_ScalingMode key.

## Topics

### Scaling Modes

let kVTScalingMode_Normal: CFString

The full width and height of the source image buffer is stretched to the full width and height of the destination image buffer.

let kVTScalingMode_CropSourceToCleanAperture: CFString

The source image buffer’s clean aperture is scaled to the destination clean aperture.

let kVTScalingMode_Letterbox: CFString

The source image buffer’s clean aperture is scaled to a rectangle fitted inside the destination clean aperture that preserves the source picture aspect ratio.

let kVTScalingMode_Trim: CFString

The source image buffer’s clean aperture is scaled to a rectangle that completely fills the destination clean aperture and preserves the source picture aspect ratio.

## See Also

### Configuration

let kVTPixelTransferPropertyKey_ScalingMode: CFString

Scaling mode for images during transfer between source and destination buffers.

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

