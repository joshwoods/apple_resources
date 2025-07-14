

- SceneKit
-  SCNPhysicsWorld 

Class

# SCNPhysicsWorld

The global simulation of collisions, gravity, joints, and other physics effects in a scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNPhysicsWorld
```

## Overview

You do not create SCNPhysicsWorld objects directly; instead, read the physicsWorld property of an SCNScene object. Use physics world object to perform the following tasks:

- Manage global properties of the simulation, such as its speed and constant gravity. (For more precise control of gravity and similar effects, see the SCNPhysicsField class.)

- Register behaviors that modify interactions between the scene’s physics bodies, such as joints and vehicles. For more details, see SCNPhysicsBehavior.

- Specify a delegate object to receive messages when two physics bodies contact each other

- Perform specific contact tests, and search for physics bodies in the scene using ray and sweep tests.

## Topics

### Managing the Physics Simulation

var gravity: SCNVector3

A vector that specifies the gravitational acceleration applied to physics bodies in the physics world.

var speed: CGFloat

The rate at which the simulation executes.

var timeStep: TimeInterval

The time interval between updates to the physics simulation.

func updateCollisionPairs()

Forces the physics engine to reevaluate possible collisions between physics bodies.

### Registering Physics Behaviors

func addBehavior(SCNPhysicsBehavior)

Adds a behavior to the physics world.

func removeBehavior(SCNPhysicsBehavior)

Removes a behavior from the physics world.

var allBehaviors: [SCNPhysicsBehavior]

The list of behaviors affecting bodies in the physics world.

func removeAllBehaviors()

Removes all behaviors affecting bodies in the physics world.

### Detecting Contacts Between Physics Bodies

var contactDelegate: (any SCNPhysicsContactDelegate)?

A delegate that is called when two physics bodies come in contact with each other.

func contactTestBetween(SCNPhysicsBody, SCNPhysicsBody, options: [SCNPhysicsWorld.TestOption : Any]?) -> [SCNPhysicsContact]

Checks for contacts between two physics bodies.

func contactTest(with: SCNPhysicsBody, options: [SCNPhysicsWorld.TestOption : Any]?) -> [SCNPhysicsContact]

Checks for contacts between one physics body and any other bodies in the physics world.

### Searching for Physics Bodies

func rayTestWithSegment(from: SCNVector3, to: SCNVector3, options: [SCNPhysicsWorld.TestOption : Any]?) -> [SCNHitTestResult]

Searches for physics bodies along a line segment between two points in the physics world.

func convexSweepTest(with: SCNPhysicsShape, from: SCNMatrix4, to: SCNMatrix4, options: [SCNPhysicsWorld.TestOption : Any]?) -> [SCNPhysicsContact]

Searches for physics bodies in the space formed by moving a convex shape through the physics world.

### Search Options

struct TestOption

Keys in options dictionaries that affect how SceneKit searches for bodies in a collision, ray, or sweep test.

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
- NSObjectProtocol
- NSSecureCoding

## See Also

### Physics in a Scene

class SCNPhysicsField

An object that applies forces, such as gravitation, electromagnetism, and turbulence, to physics bodies within a certain area of effect.

class SCNPhysicsBehavior

The abstract superclass for joints, vehicle simulations, and other high-level behaviors that incorporate multiple physics bodies.

