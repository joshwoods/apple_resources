

- Video Toolbox
-  kVTScalingMode_Normal 

Global Variable

# kVTScalingMode_Normal

The full width and height of the source image buffer is stretched to the full width and height of the destination image buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTScalingMode_Normal: CFString
```

## Discussion

The source image buffer’s clean aperture and pixel aspect ratio attachments are stretched the same way as the image with the image, and attached to the destination image buffer.This is the default scaling mode.

## See Also

### Scaling Modes

let kVTScalingMode_CropSourceToCleanAperture: CFString

The source image buffer’s clean aperture is scaled to the destination clean aperture.

let kVTScalingMode_Letterbox: CFString

The source image buffer’s clean aperture is scaled to a rectangle fitted inside the destination clean aperture that preserves the source picture aspect ratio.

let kVTScalingMode_Trim: CFString

The source image buffer’s clean aperture is scaled to a rectangle that completely fills the destination clean aperture and preserves the source picture aspect ratio.

