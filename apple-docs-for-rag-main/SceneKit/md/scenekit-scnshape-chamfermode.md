

- SceneKit
- SCNShape
-  chamferMode 

Instance Property

# chamferMode

A constant specifying which ends of the extruded shape’s profile are chamfered.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var chamferMode: SCNChamferMode { get set }
```

## Discussion

See SCNChamferMode for allowed values. The default chamfer mode is SCNChamferMode.both.

## See Also

### Chamfering a Shape

enum SCNChamferMode

Options for which edges of an extruded shape are chamfered, used by the chamferMode property.

var chamferProfile: UIBezierPath?

A path that determines the cross-sectional contour of each chamfered edge.

var chamferRadius: CGFloat

The width or depth of each chamfered edge. Animatable.

