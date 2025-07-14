

- SceneKit
- SCNPhysicsShape
- SCNPhysicsShape.Option
-  keepAsCompound 

Type Property

# keepAsCompound

An option for selecting whether to create a group of independent shapes or combine them into a single shape.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let keepAsCompound: SCNPhysicsShape.Option
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value. The default value is true, specifying that SceneKit convert separate geometries into separate shapes and join the resulting shapes. If false, SceneKit creates a single shape approximating the combined form of the geometries.

## See Also

### Type Properties

static let collisionMargin: SCNPhysicsShape.Option

static let scale: SCNPhysicsShape.Option

An option for selecting the scale factor of the shape relative to the local coordinate space of the node containing it.

static let type: SCNPhysicsShape.Option

An option for selecting the level of detail at which to create shapes from geometry.

struct ShapeType

Values for the type key specifying the level of detail that SceneKit uses when creating a physics shape based on a geometry.

