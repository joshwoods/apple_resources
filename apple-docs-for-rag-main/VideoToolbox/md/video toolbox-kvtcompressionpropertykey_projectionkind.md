

- Video Toolbox
-  kVTCompressionPropertyKey_ProjectionKind 

Global Variable

# kVTCompressionPropertyKey_ProjectionKind

A value that indicates the projection kind.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
let kVTCompressionPropertyKey_ProjectionKind: CFString
```

## Discussion

The value will be set on the format description (`kCMFormatDescriptionExtension_ProjectionKind`) for output samples and may affect the decoded frame presentation.

## See Also

### Video Extended Usage (VEXU) Signaling

let kVTCompressionPropertyKey_HeroEye: CFString

A value that indicates which eye is the primary eye when rendering in 2D.

let kVTCompressionPropertyKey_StereoCameraBaseline: CFString

A value that specifies the distance between centers of the lenses of the camera system.

let kVTCompressionPropertyKey_HorizontalDisparityAdjustment: CFString

A value that indicates a relative shift of the left and right images, which changes the zero parallax plane.

let kVTCompressionPropertyKey_ViewPackingKind: CFString

A value that indicates the view packing kind.

