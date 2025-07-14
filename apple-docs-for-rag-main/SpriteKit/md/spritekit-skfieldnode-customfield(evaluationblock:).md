

- SpriteKit
- SKFieldNode
-  customField(evaluationBlock:) 

Type Method

# customField(evaluationBlock:)

Creates a field node that calculates and applies a custom force to the physics body.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
class func customField(evaluationBlock block: @escaping SKFieldForceEvaluator) -> SKFieldNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class func customField(evaluationBlock block: @escaping SKFieldForceEvaluator) -> SKFieldNode
```

## Parameters 

`block`  

A custom block to be executed when a physics body is affected by the field. Your block should calculate and return the force to be applied to the body.

## Return Value

A new custom field node.

## Discussion

The value returned by the custom block is a vector for an impulse force which is applied to the physics body being evaluated for that frame. Only the `x` and `y` components of the return value are used by SpriteKit, the `z` component is ignored.

The values passed into the block by the `position` and `velocity` arguments measured in meters: if you need to convert them into points — as used by SpriteKit — multiply the values by 150.

The following code shows how to create a custom field to emulate drag. The block returns the negative of the square root of the velocity of the physics body. This decelerates a physics body passing through the SKFieldNode object’s region.

Listing 1. Creating a custom drag field

```
let simpleDrag = SKFieldNode.customField {
    (position: vector_float3, velocity: vector_float3, mass: Float, charge: Float, deltaTime: TimeInterval) in
    return vector_float3(-sqrt(abs(velocity.x)) * sign(velocity.x),
                         -sqrt(abs(velocity.y)) * sign(velocity.y),
                         0)
}
```

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

class func velocityField(withVector: vector_float3) -> SKFieldNode

Creates a field node that gives physics bodies a constant velocity.

class func vortexField() -> SKFieldNode

Creates a field node that applies a perpendicular force to physics bodies.

typealias SKFieldForceEvaluator

The definition for a custom block that processes a single physics body’s interaction with the field.

