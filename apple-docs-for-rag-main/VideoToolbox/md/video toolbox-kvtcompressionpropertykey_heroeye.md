

- Video Toolbox
-  kVTCompressionPropertyKey_HeroEye 

Global Variable

# kVTCompressionPropertyKey_HeroEye

A value that indicates which eye is the primary eye when rendering in 2D.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_HeroEye: CFString
```

## Discussion

This property sets a value for the kCMFormatDescriptionExtension_HeroEye format description on the output samples. Supported values are kCMFormatDescriptionHeroEye_Left or kCMFormatDescriptionHeroEye_Right.

## See Also

### Video Extended Usage (VEXU) Signaling

let kVTCompressionPropertyKey_StereoCameraBaseline: CFString

A value that specifies the distance between centers of the lenses of the camera system.

let kVTCompressionPropertyKey_HorizontalDisparityAdjustment: CFString

A value that indicates a relative shift of the left and right images, which changes the zero parallax plane.

let kVTCompressionPropertyKey_ProjectionKind: CFString

A value that indicates the projection kind.

let kVTCompressionPropertyKey_ViewPackingKind: CFString

A value that indicates the view packing kind.

