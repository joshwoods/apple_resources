

- SceneKit
- SCNPhysicsField
-  offset 

Instance Property

# offset

The offset of the field’s center within its area of effect.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var offset: SCNVector3 { get set }
```

## Discussion

Some types of fields apply forces whose magnitude is relative to the distance between an object and the field’s center. (For details on each type of field, see the methods listed in Creating Physics Fields.) Changing the offset changes the effects of these field types.

With the default offset vector `{0, 0, 0}`, the center of a field is the center of its area of effect.

## See Also

### Specifying a Field’s Area of Effect

var halfExtent: SCNVector3

A location marking the end of the field’s area of effect.

var scope: SCNPhysicsFieldScope

The area affected by the field, either inside or outside its region.

var usesEllipsoidalExtent: Bool

A Boolean value that determines whether the field’s area of effect is shaped like a box or ellipsoid.

var direction: SCNVector3

The field’s directional axis.

