

- SpriteKit
- SKFieldNode
-  linearGravityField(withVector:) 

Type Method

# linearGravityField(withVector:)

Creates a field node that accelerates physics bodies in a specific direction.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class func linearGravityField(withVector direction: vector_float3) -> SKFieldNode
```

**watchOS**

``` source
class func linearGravityField(withVector direction: vector_float3) -> SKFieldNode
```

## Parameters 

`direction`  

The direction and magnitude of the gravitational force. The values represent the acceleration of the field in meters per second squared. For example, to simulate earth’s gravity, specify `(0, -9.8, 0)`. The `z` component on the vector is ignored.

## Return Value

A new linear gravity field node.

## Discussion

If the field node is rotated, the direction of its gravity field is also rotated. The calculated force is proportional to the physics body’s mass (meaning that the acceleration applied to all affected physics bodies is a constant).

## See Also

### Creating Field Nodes

class func dragField() -> SKFieldNode

Creates a field node that applies a force that resists the motion of physics bodies.

class func electricField() -> SKFieldNode

Creates a field node that applies an electrical force proportional to the electrical charge of physics bodies.

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

class func velocityField(withVector: vector_float3) -> SKFieldNode

Creates a field node that gives physics bodies a constant velocity.

class func vortexField() -> SKFieldNode

Creates a field node that applies a perpendicular force to physics bodies.

class func customField(evaluationBlock: SKFieldForceEvaluator) -> SKFieldNode

Creates a field node that calculates and applies a custom force to the physics body.

typealias SKFieldForceEvaluator

The definition for a custom block that processes a single physics body’s interaction with the field.

