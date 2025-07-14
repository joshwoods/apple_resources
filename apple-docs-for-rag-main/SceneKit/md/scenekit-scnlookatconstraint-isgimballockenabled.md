

- SceneKit
- SCNLookAtConstraint
-  isGimbalLockEnabled 

Instance Property

# isGimbalLockEnabled

A Boolean value that specifies whether constrained nodes are allowed to rotate.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var isGimbalLockEnabled: Bool { get set }
```

## Discussion

If the value of this property is true, constrained nodes are limited in rotation around a roll axis (the vector pointing from the constrained node to the target node). If the value of this property is false (the default), constrained nodes rotate freely around this axis when the constraint adjusts their orientation.

For example, when constraining a camera to follow a moving object, setting this property to true ensures that the horizon remains level from the camera’s point of view.

## See Also

### Modifying a Constraint

var target: SCNNode?

The node toward which constrained nodes will point after being reoriented.

