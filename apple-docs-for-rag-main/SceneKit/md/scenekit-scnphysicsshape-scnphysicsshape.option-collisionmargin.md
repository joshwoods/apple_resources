

- SceneKit
- SCNPhysicsShape
- SCNPhysicsShape.Option
-  collisionMargin 

Type Property

# collisionMargin

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static let collisionMargin: SCNPhysicsShape.Option
```

## See Also

### Type Properties

static let keepAsCompound: SCNPhysicsShape.Option

An option for selecting whether to create a group of independent shapes or combine them into a single shape.

static let scale: SCNPhysicsShape.Option

An option for selecting the scale factor of the shape relative to the local coordinate space of the node containing it.

static let type: SCNPhysicsShape.Option

An option for selecting the level of detail at which to create shapes from geometry.

struct ShapeType

Values for the type key specifying the level of detail that SceneKit uses when creating a physics shape based on a geometry.

