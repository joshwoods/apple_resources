

- SceneKit
- SCNPhysicsShape
- SCNPhysicsShape.Option
-  type 

Type Property

# type

An option for selecting the level of detail at which to create shapes from geometry.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let type: SCNPhysicsShape.Option
```

## Discussion

The value for this key is one of the constants listed in `Shape Types`. The default type is convexHull.

## See Also

### Type Properties

static let collisionMargin: SCNPhysicsShape.Option

static let keepAsCompound: SCNPhysicsShape.Option

An option for selecting whether to create a group of independent shapes or combine them into a single shape.

static let scale: SCNPhysicsShape.Option

An option for selecting the scale factor of the shape relative to the local coordinate space of the node containing it.

struct ShapeType

Values for the type key specifying the level of detail that SceneKit uses when creating a physics shape based on a geometry.

