

- SceneKit
- SCNShape
-  chamferProfile 

Instance Property

# chamferProfile

A path that determines the cross-sectional contour of each chamfered edge.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
@NSCopying
var chamferProfile: UIBezierPath? { get set }
```

**macOS**

``` source
@NSCopying
var chamferProfile: NSBezierPath? { get set }
```

## Discussion

The value of this property must be a two-dimensional path starting at the point `{1, 0}` and ending at the point `{0, 1}`, determining the contour of the shape along its extruded sides, as illustrated in the figure below. If the value of this property is `nil` and the value of the chamferRadius property is greater than zero, SceneKit uses a chamfer profile in the shape of a quarter circle.

## See Also

### Chamfering a Shape

var chamferMode: SCNChamferMode

A constant specifying which ends of the extruded shape’s profile are chamfered.

enum SCNChamferMode

Options for which edges of an extruded shape are chamfered, used by the chamferMode property.

var chamferRadius: CGFloat

The width or depth of each chamfered edge. Animatable.

