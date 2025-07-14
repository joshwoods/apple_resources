

- SceneKit
- SCNPhysicsShape
-  SCNPhysicsShape.ShapeType 

Structure

# SCNPhysicsShape.ShapeType

Values for the type key specifying the level of detail that SceneKit uses when creating a physics shape based on a geometry.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct ShapeType
```

## Topics

### Type Properties

static let boundingBox: SCNPhysicsShape.ShapeType

The physics shape is the smallest box containing the geometry.

static let concavePolyhedron: SCNPhysicsShape.ShapeType

The physics shape is a concave polyhedron closely following the surface of the geometry.

static let convexHull: SCNPhysicsShape.ShapeType

The physics shape is a convex polyhedron roughly enclosing the geometry.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Type Properties

static let collisionMargin: SCNPhysicsShape.Option

static let keepAsCompound: SCNPhysicsShape.Option

An option for selecting whether to create a group of independent shapes or combine them into a single shape.

static let scale: SCNPhysicsShape.Option

An option for selecting the scale factor of the shape relative to the local coordinate space of the node containing it.

static let type: SCNPhysicsShape.Option

An option for selecting the level of detail at which to create shapes from geometry.

