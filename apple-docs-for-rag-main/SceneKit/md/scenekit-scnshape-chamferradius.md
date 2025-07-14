

- SceneKit
- SCNShape
-  chamferRadius 

Instance Property

# chamferRadius

The width or depth of each chamfered edge. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var chamferRadius: CGFloat { get set }
```

## Discussion

The default value of zero specifies no chamfer (the extruded sides end at right angles to the front and back of the shape). Allowed values range from zero to half the extrusion depth. (At the maximum chamfer radius, the front chamfer ends where the back chamfer begins, as shown on the right in the figure below.)

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Chamfering a Shape

var chamferMode: SCNChamferMode

A constant specifying which ends of the extruded shape’s profile are chamfered.

enum SCNChamferMode

Options for which edges of an extruded shape are chamfered, used by the chamferMode property.

var chamferProfile: UIBezierPath?

A path that determines the cross-sectional contour of each chamfered edge.

