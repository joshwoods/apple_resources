

- SpriteKit
-  SKFieldNode 

Class

# SKFieldNode

A node that applies physics effects to nearby nodes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
class SKFieldNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
class SKFieldNode
```

## Mentioned in 

Getting Started with Physics

Adding Physics Fields to a Scene

## Overview

There are many different kinds of field nodes that can be created, each with different effects. The SKFieldNode section lists the field types you can create using SpriteKit, including a type that allows you to apply custom forces to physics bodies. Instantiate the appropriate kind of field node and then add it to the scene’s node tree.

When the scene simulates physics effects, a field node applies its effect to a physics body so long as the following are true:

- The field node is in the scene’s node tree.

- The field node’s isEnabled property is true.

- The physics body is attached to a node that is in the scene’s node tree.

- The physics body is located inside the field node’s region (see region).

- The physics body is not located inside the region of another field node whose isExclusive property is set to true.

- A logical AND operation between the field node’s categoryBitMask property and the physics body’s fieldBitMask property results in a nonzero value.

Tip

While it is useful to know that SpriteKit measures items in the International System of Units, the precise numbers are not that important. It doesn’t matter much whether your rocket ship weights 1 kilogram or 1,000,000 kilograms, as long as the mass is consistent with other physics values used in the game. Often, proportions are more important than the actual values being used.

## Topics

### Getting Started with Field Nodes

Adding Physics Fields to a Scene

Create effects that interact with your scene’s physics bodies, such as magnetism, repulsion, friction, or a vortex.

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

typealias SKFieldForceEvaluator

The definition for a custom block that processes a single physics body’s interaction with the field.

### Determining Which Physics Bodies Are Affected by the Field

var isEnabled: Bool

A Boolean value that indicates whether the field is active.

var isExclusive: Bool

A Boolean value that indicates whether the field node should override all other field nodes that might otherwise affect physics bodies.

var region: SKRegion?

The area (relative to the node’s origin) that the field affects.

var minimumRadius: Float

The minimum value for distance-based effects.

var categoryBitMask: UInt32

A mask that defines which categories this field belongs to.

### Configuring the Strength of the Field

var strength: Float

The strength of the field.

var falloff: Float

The exponent that defines the rate of decay for the strength of the field as the distance increases between the node and the physics body being affected.

### Configuring Other Field Properties

These properties are associated with specific types of field nodes.

var animationSpeed: Float

The rate at which a noise or turbulence field node changes.

var smoothness: Float

The smoothness of the noise used to generate the forces.

var direction: vector_float3

The direction of a velocity field node.

var texture: SKTexture?

A normal texture that specifies the velocities at different points in a velocity field node.

## Relationships

### Inherits From

- SKNode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- Sendable
- UIActivityItemsConfigurationProviding
- UICoordinateSpace
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Physics Simulation

Getting Started with Physics

Simulate gravity, acceleration, collision detection, or joints.

class SKPhysicsWorld

The driver of the physics engine in a scene; it exposes the ability for you to configure and query the physics system.

class SKPhysicsBody

An object that adds physics simulation to a node.

class SKPhysicsContact

A description of the contact between two physics bodies.

protocol SKPhysicsContactDelegate

Methods your app can implement to respond when physics bodies come into contact.

