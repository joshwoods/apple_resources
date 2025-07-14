

- SceneKit
-  SCNPhysicsBody 

Class

# SCNPhysicsBody

The physics simulation attributes attached to a scene graph node.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNPhysicsBody
```

## Overview

When SceneKit prepares to render a new frame, it performs physics calculations on physics bodies attached to nodes in the scene. These calculations include gravity, friction, and collisions with other bodies. You can also apply your own forces and impulses to a body. After SceneKit completes these calculations, it updates the positions and orientations of the node objects before rendering the frame.

To add physics to a node, create and configure an SCNPhysicsBody object and then assign it to the physicsBody property of the SCNNode object. A physics body must be associated with a node object before you apply forces or impulses to it.

### A Body’s Physical Characteristics

The SCNPhysicsBody class defines the physical characteristics for the body when it is simulated by the scene. Three properties are most important for physics simulation:

- The type property, which determines how the body interacts with forces and other bodies in the simulation. *Static* bodies are unaffected by forces and collisions and cannot move. *Dynamic* bodies are affected by forces and collisions with other body types. *Kinematic* bodies are not affected by forces or collisions, but by moving them directly you can cause collisions that affect dynamic bodies.

- The physicsShape property, which defines the three-dimensional form of the body for collision detection purposes. Physics simulations run faster when using simple shapes instead of the fine detail of a node’s visible geometry. Typically, you set a body’s physics shape to a bounding box, sphere, or primitive shape that roughly matches its node’s visible content. For details on creating physics shapes, see SCNPhysicsShape.

- The kinematic() property. Applying a force or torque to a dynamic body results in an acceleration (or angular acceleration) proportional to its mass.

All values in SceneKit’s physics simulation use the International System of Units (SI): The unit of mass is the kilogram; the units of force, impulse, and torque are the newton, newton-second, and newton-meter; and the unit of distance for node positions and sizes is the meter. Note that you need not attempt to provide realistic values for physical quantities—use whatever values produce the behavior or gameplay you’re looking for.

For a dynamic body, you can control how the body is affected by forces or collisions. See Defining How Forces Affect a Physics Body.

### Defining a Body’s Category and Collisions

When you design a game that uses physics, you define the different categories of physics objects that appear in the scene. You define different categories of physics bodies for the behaviors your want for your app. A body can be assigned to as many of these categories as you want. In addition to declaring its own categories, a physics body also declares which categories of bodies it interacts with.

Use the categoryBitMask and collisionBitMask properties to define an object’s collision behavior. The constants listed in SCNPhysicsCollisionCategory provide default values for these properties. In addition, with the contactTestBitMask property you can define interactions where a pair of bodies generates contact messages (see the SCNPhysicsContactDelegate protocol) without the bodies being affected by the collision.

### Related Physics Classes

Physics fields create forces that affect all bodies in an area, such as vortices and gravitational attraction. For details and a list of available field types, see SCNPhysicsField.

You can add higher-level behaviors that control interactions between multiple bodies, such as joints and wheeled vehicles. For details and a list of available behaviors, see SCNPhysicsBehavior.

A scene’s physicsWorld property holds an SCNPhysicsWorld object that manages physics characteristics that affect the entire scene.

### Physics and the Rendering Loop

SceneKit evaluates its physics simulation as part of the rendering loop described in SCNSceneRendererDelegate. On each pass through this loop, SceneKit determines the state of all nodes with attached physics bodies, and simulates the effects of physics on those bodies for one time step—for example, by updating the position or rotation of a body based on its velocity and angular velocity. After simulating physics, SceneKit applies the results of the physics simulation to the scene for display.

Because you can animate SceneKit content not only through physics, but also through actions and implicitly and explicitly defined animations, SceneKit applies the results of physics simulation not to the SCNNode objects in your scene, but to each node’s presentation object that represents its currently displayed state. As such, changing properties of a node that are affected by physics requires special consideration.

If you change the transform value—or any of the other properties that are components of the transform, such as position and rotation—of a node affected by physics, SceneKit resets the physics simulation for that node. If you want to change only one component of the transform, while leaving the others at their physics-simulated values, copy the presentation node’s transform before making changes, as shown below:

- Swift
- Objective-C

```
// Copy the presentation node's transform to the model node.
node.transform = node.presentationNode.transform
// Change one component of the new transform
node.eulerAngles.z = newRollValue
```

```
// Copy the presentation node's transform to the model node.
node.transform = node.presentationNode.transform;
// Change one component of the new transform
node.eulerAngles = SCNVector3Make(node.eulerAngles.x, node.eulerAngles.y, newRollValue);
```

## Topics

### Creating Physics Bodies

convenience init(type: SCNPhysicsBodyType, shape: SCNPhysicsShape?)

Creates a physics body with the specified type and shape.

class func `static`() -> Self

Creates a physics body that is unaffected by forces or collisions and that cannot move.

class func dynamic() -> Self

Creates a physics body that can be affected by forces and collisions.

class func kinematic() -> Self

Creates a physics body that is unaffected by forces or collisions but that can cause collisions affecting other bodies when moved.

### Defining How Forces Affect a Physics Body

var physicsShape: SCNPhysicsShape?

An object that defines the solid volume of the physics body for use in collision detection.

var type: SCNPhysicsBodyType

A constant that determines how the physics body responds to forces and collisions.

enum SCNPhysicsBodyType

Constants that determine how a physics body interacts with forces and other bodies, used by the type property and when creating a physics body.

var velocityFactor: SCNVector3

A multiplier affecting how SceneKit applies translations computed by the physics simulation to the node containing the physics body.

var angularVelocityFactor: SCNVector3

A multiplier affecting how SceneKit applies rotations computed by the physics simulation to the node containing the physics body.

var isAffectedByGravity: Bool

A Boolean value that determines whether the constant gravity of a scene accelerates the body.

### Defining a Body’s Physical Properties

var mass: CGFloat

The mass of the body, in kilograms.

var charge: CGFloat

The electric charge of the body, in coulombs.

var friction: CGFloat

The body’s resistance to sliding motion.

var rollingFriction: CGFloat

The body’s resistance to rolling motion.

var restitution: CGFloat

A factor that determines how much kinetic energy the body loses or gains in collisions.

var damping: CGFloat

A factor that reduces the body’s linear velocity.

var angularDamping: CGFloat

A factor that reduces the body’s angular velocity.

var momentOfInertia: SCNVector3

The body’s moment of inertia, expressed in the local coordinate system of the node that contains the body.

var usesDefaultMomentOfInertia: Bool

A Boolean value that determines whether SceneKit automatically calculates the body’s moment of inertia or allows setting a custom value.

var centerOfMassOffset: SCNVector3

The position of the body’s center of mass relative to its local coordinate origin.

### Working with Contacts and Collisions

var categoryBitMask: Int

A mask that defines which categories this physics body belongs to.

var contactTestBitMask: Int

A mask that defines which categories of bodies cause intersection notifications with this physics body.

var collisionBitMask: Int

A mask that defines which categories of physics bodies can collide with this physics body.

struct SCNPhysicsCollisionCategory

Default values for a physics body’s categoryBitMask and collisionBitMask properties.

var continuousCollisionDetectionThreshold: CGFloat

The minimum distance the body must travel for SceneKit to apply a more precise (but more costly) algorithm to detect contacts with other bodies.

### Applying Forces, Impulses, and Torques

func applyForce(SCNVector3, asImpulse: Bool)

Applies a force or impulse to the body at its center of mass.

func applyForce(SCNVector3, at: SCNVector3, asImpulse: Bool)

Applies a force or impulse to the body at a specific point.

func applyTorque(SCNVector4, asImpulse: Bool)

Applies a net torque or a change in angular momentum to the body.

func clearAllForces()

Cancels all continuous forces and torques acting on the physics body during the current simulation step.

### Interacting with Bodies in Motion

var velocity: SCNVector3

A vector describing both the current speed (in meters per second) and direction of motion of the physics body.

var angularVelocity: SCNVector4

A vector describing both the current rotation axis and rotational speed (in radians per second) of the physics body.

### Defining When a Body Can Move

var isResting: Bool

A Boolean value that indicates whether the physics body is at rest.

var allowsResting: Bool

A Boolean value that specifies whether SceneKit can automatically mark the physics body at rest.

func setResting(Bool)

Tells SceneKit whether to treat the body as currently being in motion.

### Synchronizing a Physics Body with its Node

func resetTransform()

Updates the position and orientation of a body in the physics simulation to match that of the node to which the body is attached.

### Instance Properties

var angularRestingThreshold: CGFloat

var linearRestingThreshold: CGFloat

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

### Physics Bodies

class SCNPhysicsShape

An abstraction of a physics body’s solid volume for tuning collision detection.

