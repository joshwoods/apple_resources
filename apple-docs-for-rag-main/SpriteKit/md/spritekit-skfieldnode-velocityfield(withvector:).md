

- SpriteKit
- SKFieldNode
-  velocityField(withVector:) 

Type Method

# velocityField(withVector:)

Creates a field node that gives physics bodies a constant velocity.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
class func velocityField(withVector direction: vector_float3) -> SKFieldNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class func velocityField(withVector direction: vector_float3) -> SKFieldNode
```

## Parameters 

`direction`  

The velocity that any affected physics bodies will have. The `z` component on the vector is ignored.

## Return Value

A new velocity field node.

## See Also

### Creating Field Nodes

class func dragField() -> SKFieldNode

Creates a field node that applies a force that resists the motion of physics bodies.

class func electricField() -> SKFieldNode

Creates a field node that applies an electrical force proportional to the electrical charge of physics bodies.

class func linearGravityField(withVector: vector_float3) -> SKFieldNode

Creates a field node that accelerates physics bodies in a specific direction.

class func magneticField() -> SKFieldNode

Creates a field node that applies a magnetic force based on the velocity and electrical charge of the physics bodies.

class func noiseField(withSmoothness: CGFloat, animationSpeed: CGFloat) -> SKFieldNode

Creates a field node that applies a randomized acceleration to physics bodies.

class func radialGravityField() -> SKFieldNode

Creates a field node that accelerates physics bodies toward the field node.

class func springField() -> SKFieldNode

Creates a field node that applies a spring-like force that pulls physics bodies toward the field node.

class func turbulenceField(withSmoothness: CGFloat, animationSpeed: CGFloat) -> SKFieldNode

Creates a field node that applies a randomized acceleration to physics bodies.

class func velocityField(with: SKTexture) -> SKFieldNode

Creates a field node that sets the velocity of physics bodies that enter the node’s area based on the pixel values of a texture.

class func vortexField() -> SKFieldNode

Creates a field node that applies a perpendicular force to physics bodies.

class func customField(evaluationBlock: SKFieldForceEvaluator) -> SKFieldNode

Creates a field node that calculates and applies a custom force to the physics body.

typealias SKFieldForceEvaluator

The definition for a custom block that processes a single physics body’s interaction with the field.

