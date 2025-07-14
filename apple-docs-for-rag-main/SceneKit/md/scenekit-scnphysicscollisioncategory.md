

- SceneKit
-  SCNPhysicsCollisionCategory 

Structure

# SCNPhysicsCollisionCategory

Default values for a physics body’s categoryBitMask and collisionBitMask properties.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
struct SCNPhysicsCollisionCategory
```

## Overview

You specify contact and collision behaviors by defining your own categories for the kinds of bodies your app simulates and setting the categoryBitMask and collisionBitMask properties for each body to determine which kinds of bodies it collides with. Additionally, you can use the contactDelegate property of the physics world to be notified of collisions between bodies.

For more details and example usage, see Defining a Body’s Category and Collisions in the class overview.

## Topics

### Constants

static var `default`: SCNPhysicsCollisionCategory

The default categoryBitMask value for dynamic and kinematic bodies.

static var `static`: SCNPhysicsCollisionCategory

The default categoryBitMask value for static bodies.

static var all: SCNPhysicsCollisionCategory

This is the default value for a physics body’s collisionBitMask property.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Working with Contacts and Collisions

var categoryBitMask: Int

A mask that defines which categories this physics body belongs to.

var contactTestBitMask: Int

A mask that defines which categories of bodies cause intersection notifications with this physics body.

var collisionBitMask: Int

A mask that defines which categories of physics bodies can collide with this physics body.

var continuousCollisionDetectionThreshold: CGFloat

The minimum distance the body must travel for SceneKit to apply a more precise (but more costly) algorithm to detect contacts with other bodies.

