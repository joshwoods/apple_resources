

- SpriteKit
-  SKPhysicsBody 

Class

# SKPhysicsBody

An object that adds physics simulation to a node.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class SKPhysicsBody
```

## Mentioned in 

Getting Started with Physics

Getting Started with Physics Bodies

Responding to Frame-Cycle Events

## Overview

Assign a SKPhysicsBody object to the physicsBody property of the SKNode object to add physics simulation to the node. When a scene processes a new frame, it performs physics calculations on physics bodies attached to nodes in the scene. These calculations include gravity, friction, and collisions with other bodies. You can also apply your own forces and impulses to a body. After the scene completes these calculations, it updates the positions and orientations of the node objects.

Important

A physics body must be associated with a node before you apply forces or impulses to it.

SpriteKit supports two kinds of physics bodies, *volume-based bodies* and *edge-based bodies*. When you create a physics body, its kind, size, and shape are determined by the constructor method you call. An edge-based body does not have mass or volume and is unaffected by forces or impulses in the system. Edge-based bodies are used to represent volumeless boundaries or hollow spaces in your physics simulation. In contrast, volume-based bodies are used to represent objects with mass and volume. The isDynamic property controls whether a volume-based body is affected by gravity, friction, collisions with other objects, and forces or impulses you directly apply to it.

The SKPhysicsBody class defines the physical characteristics for the body when it is simulated by the scene. For volume-based bodies, the most important property is the mass property. A volume-based body is assumed to have a uniform density. You can either set the mass property directly, or you can set the body’s density property and let the physics body calculate its own mass. All values in Sprite Kit are specified using the International System of Units (SI units). The actual forces and mass values are not important so long as your game uses consistent values.

When you design a game that uses physics, you define the different categories of physics objects that appear in the scene. You define up to 32 different categories of physics bodies, and a body can be assigned to as many of these categories as you want. In addition to declaring its own categories, a physics body also declares which categories of bodies it interacts with. See SKPhysicsBody. You use a similar mechanism to declare which physics field nodes (SKFieldNode) can affect the physics body.

For a volume-based body, you can dynamically control how the body is affected by forces or collisions. See SKPhysicsBody.

## Topics

### First Steps

Getting Started with Physics Bodies

Create and assign a physics body to enable physics.

### Creating a Body from a Shape

init(circleOfRadius: CGFloat)

Creates a circular physics body centered on the owning node’s origin.

init(circleOfRadius: CGFloat, center: CGPoint)

Creates a circular physics body centered on an arbitrary point.

init(rectangleOf: CGSize)

Creates a rectangular physics body centered on the owning node’s origin.

init(rectangleOf: CGSize, center: CGPoint)

Creates a rectangular physics body centered on an arbitrary point.

init(polygonFrom: CGPath)

Creates a polygonal physics body.

### Creating a Body from a Texture

Shaping a Physics Body to Match a Node’s Graphics

Shape a physics body to your graphics for the right blend of collision accuracy and performance.

init(texture: SKTexture, size: CGSize)

Creates a physics body from the contents of a texture.

init(texture: SKTexture, alphaThreshold: Float, size: CGSize)

Creates a physics body from the contents of a texture, capturing only the texels that exceed a specified transparency value.

### Creating a Body from a Collection of Bodies

init(bodies: [SKPhysicsBody])

Creates a physics body that’s shaped like a union of the argument physics bodies.

### Creating an Edge-Based Physics Body

Creating an Edge Loop Around a Scene

Border your scene with an obstacle that physics bodies cannot penetrate.

init(edgeLoopFrom: CGRect)

Creates an edge loop from a rectangle.

init(edgeFrom: CGPoint, to: CGPoint)

Creates an edge between two points.

init(edgeLoopFrom: CGPath)

Creates an edge loop from a path.

init(edgeChainFrom: CGPath)

Creates an edge chain from a path.

### Defining How Forces Affect a Physics Body

var affectedByGravity: Bool

A Boolean value that indicates whether this physics body is affected by the physics world’s gravity.

var allowsRotation: Bool

A Boolean value that indicates whether the physics body is affected by angular forces and impulses applied to it.

var isDynamic: Bool

A Boolean value that indicates whether the physics body is moved by the physics simulation.

### Defining a Physics Body’s Physical Properties

Configuring a Physics Body

Move a physics body, and make it collide with other objects, by setting its physical properties once or changing them dynamically.

var mass: CGFloat

The mass of the body, in kilograms.

var density: CGFloat

The density of the object, in kilograms per square meter.

var area: CGFloat

The area covered by the body.

var friction: CGFloat

The roughness of the surface of the physics body.

var restitution: CGFloat

The bounciness of the physics body.

var linearDamping: CGFloat

A property that reduces the body’s linear velocity.

var angularDamping: CGFloat

A property that reduces the body’s rotational velocity.

### Working with Collisions and Contacts

About Collisions and Contacts

Learn how to set up nodes for collision detection.

var categoryBitMask: UInt32

A mask that defines which categories this physics body belongs to.

var collisionBitMask: UInt32

A mask that defines which categories of physics bodies can collide with this physics body.

var usesPreciseCollisionDetection: Bool

A Boolean value that determines whether the physics world uses an iterative collision detection algorithm.

var contactTestBitMask: UInt32

A mask that defines which categories of physics bodies cause intersection notifications with this physics body.

func allContactedBodies() -> [SKPhysicsBody]

The physics bodies that this physics body is in contact with.

### Applying Forces and Impulses to a Physics Body

Making Physics Bodies Move

Move a body using various physics properties, like velocity, gravity or impulses.

func applyForce(CGVector)

Applies a force to the center of gravity of a physics body.

func applyTorque(CGFloat)

Applies torque to an object.

func applyForce(CGVector, at: CGPoint)

Applies a force to a specific point of a physics body.

func applyImpulse(CGVector)

Applies an impulse to the center of gravity of a physics body.

func applyAngularImpulse(CGFloat)

Applies an impulse that imparts angular momentum to an object.

func applyImpulse(CGVector, at: CGPoint)

Applies an impulse to a specific point of a physics body.

### Inspecting a Physics Body’s Position and Velocity

var velocity: CGVector

The physics body’s velocity vector, measured in meters per second.

var angularVelocity: CGFloat

The physics body’s angular speed.

var isResting: Bool

A Boolean property that indicates whether the object is at rest within the physics simulation.

### Reading a Physics Body’s Node

var node: SKNode?

The node that this body is connected to.

### Determining Which Joints Are Connected to a Physics Body

var joints: [SKPhysicsJoint]

The joints connected to this physics body.

### Interacting with Physics Fields

var fieldBitMask: UInt32

A mask that defines which categories of physics fields can exert forces on this physics body.

var charge: CGFloat

The electrical charge of the physics body.

### Pinning a Physics Body to a Node’s Parent

Pinning and Rotating Physics Bodies

Pin a node so it’s free to rotate about a certain point on its parent node.

var pinned: Bool

A Boolean value that indicates whether the physics body’s node is pinned to its parent node.

## Relationships

### Inherits From

- NSObject

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

## See Also

### Physics Simulation

Getting Started with Physics

Simulate gravity, acceleration, collision detection, or joints.

class SKPhysicsWorld

The driver of the physics engine in a scene; it exposes the ability for you to configure and query the physics system.

class SKPhysicsContact

A description of the contact between two physics bodies.

protocol SKPhysicsContactDelegate

Methods your app can implement to respond when physics bodies come into contact.

class SKFieldNode

A node that applies physics effects to nearby nodes.

