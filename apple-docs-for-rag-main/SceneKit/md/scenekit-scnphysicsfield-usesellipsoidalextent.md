

- SceneKit
- SCNPhysicsField
-  usesEllipsoidalExtent 

Instance Property

# usesEllipsoidalExtent

A Boolean value that determines whether the field’s area of effect is shaped like a box or ellipsoid.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var usesEllipsoidalExtent: Bool { get set }
```

## Discussion

If this value is false (the default), the field’s area of effect is the box-shaped region of space defined by its halfExtent property and the position property of the node containing the field.

If this value is true, the field’s area of effect is the ellipsoid bounded by this box-shaped region. That is, if all components of the half-extent vector are equal, the field has a spherical area of effect.

## See Also

### Specifying a Field’s Area of Effect

var halfExtent: SCNVector3

A location marking the end of the field’s area of effect.

var scope: SCNPhysicsFieldScope

The area affected by the field, either inside or outside its region.

var offset: SCNVector3

The offset of the field’s center within its area of effect.

var direction: SCNVector3

The field’s directional axis.

