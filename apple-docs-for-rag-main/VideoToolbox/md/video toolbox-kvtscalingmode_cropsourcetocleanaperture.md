

- Video Toolbox
-  kVTScalingMode_CropSourceToCleanAperture 

Global Variable

# kVTScalingMode_CropSourceToCleanAperture

The source image buffer’s clean aperture is scaled to the destination clean aperture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTScalingMode_CropSourceToCleanAperture: CFString
```

## Discussion

The destination pixel aspect ratio is set on the destination image buffer.

## See Also

### Scaling Modes

let kVTScalingMode_Normal: CFString

The full width and height of the source image buffer is stretched to the full width and height of the destination image buffer.

let kVTScalingMode_Letterbox: CFString

The source image buffer’s clean aperture is scaled to a rectangle fitted inside the destination clean aperture that preserves the source picture aspect ratio.

let kVTScalingMode_Trim: CFString

The source image buffer’s clean aperture is scaled to a rectangle that completely fills the destination clean aperture and preserves the source picture aspect ratio.

