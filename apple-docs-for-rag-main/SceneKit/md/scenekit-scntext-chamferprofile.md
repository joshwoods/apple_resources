

- SceneKit
- SCNText
-  chamferProfile 

Instance Property

# chamferProfile

A path that determines the cross-sectional contour of each chamfered edge.

iOSiPadOSMac CatalystmacOS 10.9+tvOSvisionOSwatchOS

**macOS**

``` source
@NSCopying
var chamferProfile: NSBezierPath? { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
@NSCopying
var chamferProfile: UIBezierPath? { get set }
```

## Discussion

The value of this property must be a two-dimensional path starting at the point `{1, 0}` and ending at the point `{0, 1}`, determining the contour of the shape along its extruded sides. If the value of this property is `nil` and the value of the chamferRadius property is greater than zero, SceneKit uses a chamfer profile in the shape of a quarter circle. Figure 1 illustrates various chamfer profiles applied to the shape of a tilde (~) character.

## See Also

### Managing the Text’s 3D Representation

var flatness: CGFloat

A number that determines the accuracy or smoothness of the text geometry.

var extrusionDepth: CGFloat

The extent of the extruded text in the z-axis direction. Animatable.

var chamferRadius: CGFloat

The width or depth of each chamfered edge. Animatable.

