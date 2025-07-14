

- SceneKit
- SCNPhysicsField
-  scope 

Instance Property

# scope

The area affected by the field, either inside or outside its region.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var scope: SCNPhysicsFieldScope { get set }
```

## Discussion

First, define a field’s region using its halfExtent property and the position property of the node containing the field. Then, use the scope property to choose whether the field’s area of effect is the interior of the region (the default) or all space outside the region.

## See Also

### Specifying a Field’s Area of Effect

var halfExtent: SCNVector3

A location marking the end of the field’s area of effect.

var usesEllipsoidalExtent: Bool

A Boolean value that determines whether the field’s area of effect is shaped like a box or ellipsoid.

var offset: SCNVector3

The offset of the field’s center within its area of effect.

var direction: SCNVector3

The field’s directional axis.

