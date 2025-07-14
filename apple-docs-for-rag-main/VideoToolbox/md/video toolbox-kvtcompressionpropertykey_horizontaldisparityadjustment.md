

- Video Toolbox
-  kVTCompressionPropertyKey_HorizontalDisparityAdjustment 

Global Variable

# kVTCompressionPropertyKey_HorizontalDisparityAdjustment

A value that indicates a relative shift of the left and right images, which changes the zero parallax plane.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_HorizontalDisparityAdjustment: CFString
```

## Discussion

This property sets a value for the kCMFormatDescriptionExtension_HorizontalDisparityAdjustment format description on the output samples. The value is a 32-bit integer, measured over the range of `-10000` to `10000`, that maps to a uniform range of `-1.0` to `1.0`.

This property is optional. Only specify a disparity adjustment, including 0, when you know the specific value.

## See Also

### Video Extended Usage (VEXU) Signaling

let kVTCompressionPropertyKey_HeroEye: CFString

A value that indicates which eye is the primary eye when rendering in 2D.

let kVTCompressionPropertyKey_StereoCameraBaseline: CFString

A value that specifies the distance between centers of the lenses of the camera system.

let kVTCompressionPropertyKey_ProjectionKind: CFString

A value that indicates the projection kind.

let kVTCompressionPropertyKey_ViewPackingKind: CFString

A value that indicates the view packing kind.

