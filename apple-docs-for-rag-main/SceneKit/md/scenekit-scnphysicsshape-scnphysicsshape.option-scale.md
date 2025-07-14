

- SceneKit
- SCNPhysicsShape
- SCNPhysicsShape.Option
-  scale 

Type Property

# scale

An option for selecting the scale factor of the shape relative to the local coordinate space of the node containing it.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let scale: SCNPhysicsShape.Option
```

## Discussion

The value for this key is an NSValue object containing an SCNVector3 structure, whose components describe the scale factor in each of the x-, y- and z-axis directions. The default value is the vector `{1.0, 1.0, 1.0}`, specifying no change of scale.

SceneKit’s physics simulation ignores the scale property of nodes containing physics bodies when simulating collisions. Instead, use this option to provide a scale factor when creating custom physics shapes. (If you create a physics body for a node without specifying a custom shape, SceneKit uses the node’s scale property to infer this scale factor at creation time.)

## See Also

### Type Properties

static let collisionMargin: SCNPhysicsShape.Option

static let keepAsCompound: SCNPhysicsShape.Option

An option for selecting whether to create a group of independent shapes or combine them into a single shape.

static let type: SCNPhysicsShape.Option

An option for selecting the level of detail at which to create shapes from geometry.

struct ShapeType

Values for the type key specifying the level of detail that SceneKit uses when creating a physics shape based on a geometry.

