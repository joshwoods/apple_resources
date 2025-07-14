

- SceneKit
- SCNPhysicsShape
-  SCNPhysicsShape.Option 

Structure

# SCNPhysicsShape.Option

Keys for the options dictionary used when creating a physics shape.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct Option
```

## Discussion

When SceneKit creates a shape from a hierarchy of nodes containing multiple geometries, the keepAsCompound option takes precedence over the type option.

For example, if you have a node hierarchy containing several geometries, setting the the type option to boundingBox and the keepAsCompound option to true creates a shape that is a combination of several boxes. This approach can provide better simulation performance than converting the entire node hierarchy to a single concave polyhedron shape.

## Topics

### Type Properties

static let collisionMargin: SCNPhysicsShape.Option

static let keepAsCompound: SCNPhysicsShape.Option

An option for selecting whether to create a group of independent shapes or combine them into a single shape.

static let scale: SCNPhysicsShape.Option

An option for selecting the scale factor of the shape relative to the local coordinate space of the node containing it.

static let type: SCNPhysicsShape.Option

An option for selecting the level of detail at which to create shapes from geometry.

struct ShapeType

Values for the type key specifying the level of detail that SceneKit uses when creating a physics shape based on a geometry.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

