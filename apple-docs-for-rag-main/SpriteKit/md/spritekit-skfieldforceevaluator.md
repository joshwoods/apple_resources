

- SpriteKit
-  SKFieldForceEvaluator 

Type Alias

# SKFieldForceEvaluator

The definition for a custom block that processes a single physics body’s interaction with the field.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias SKFieldForceEvaluator = (vector_float3, vector_float3, Float, Float, TimeInterval) -> vector_float3
```

## Discussion

The block parameters are defined as follows:

position  
The position of the physics body. The coordinates are assumed to be in the following order: `x`, `y`, `z`. In SpriteKit, the `z` coordinate is always `0`.

velocity  
The velocity of the physics body. The coordinates are assumed to be in the following order: `dx`, `dy`, `dz`. In SpriteKit, the `dz` coordinate is always `0`.

mass  
The mass of the physics body.

charge  
The charge of the physics body.

time  
The amount of time that has passed since the last time the simulation was executed.

Your block should perform any force calculations you are interested in and return the resulting force.

Important

Although your app can use the z coordinate of any of the float vectors to perform its calculations, the z value of the output vector is ignored by SpriteKit. Essentially, this means that you can use field effects only to animate a node’s position property, not its zPosition property.

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

class func customField(evaluationBlock: SKFieldForceEvaluator) -> SKFieldNode

Creates a field node that calculates and applies a custom force to the physics body.

