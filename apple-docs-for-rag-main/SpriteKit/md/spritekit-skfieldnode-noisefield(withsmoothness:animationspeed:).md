

- SpriteKit
- SKFieldNode
-  noiseField(withSmoothness:animationSpeed:) 

Type Method

# noiseField(withSmoothness:animationSpeed:)

Creates a field node that applies a randomized acceleration to physics bodies.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class func noiseField(
    withSmoothness smoothness: CGFloat,
    animationSpeed speed: CGFloat
) -> SKFieldNode
```

**watchOS**

``` source
class func noiseField(
    withSmoothness smoothness: CGFloat,
    animationSpeed speed: CGFloat
) -> SKFieldNode
```

## Parameters 

`smoothness`  

The smoothness of the noise used to generate the forces. This parameter should be a value between `0.0` and `1.0`, where `1.0` represents a uniform smoothness.

`speed`  

The speed at which the noise field should change. A value of `0.0` means that the field should not animate at all.

## Return Value

A new noise field node.

## Discussion

Use a noise field to simulate effects such as fireflies or snow.

The acceleration is proportional to the field strength in a pseudo-random direction. The calculated force is proportional to the physics body’s mass (meaning that the acceleration applied to all affected physics bodies is a constant).

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

