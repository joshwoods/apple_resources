

- SceneKit
- SCNText
-  chamferRadius 

Instance Property

# chamferRadius

The width or depth of each chamfered edge. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var chamferRadius: CGFloat { get set }
```

## Discussion

A value of `0.0` (the default) or less specifies no chamfer—the extruded sides of each character end at right angles to its front and back.

The maximum chamfer radius is half the value of the extrusionDepth property. At this radius, the front chamfer ends where the back chamfer begins. However, SceneKit may automatically reduce the chamfer radius for character shapes with thin strokes.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing the Text’s 3D Representation

var flatness: CGFloat

A number that determines the accuracy or smoothness of the text geometry.

var extrusionDepth: CGFloat

The extent of the extruded text in the z-axis direction. Animatable.

var chamferProfile: UIBezierPath?

A path that determines the cross-sectional contour of each chamfered edge.

