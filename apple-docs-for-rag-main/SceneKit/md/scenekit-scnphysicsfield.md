

- SceneKit
-  SCNPhysicsField 

Class

# SCNPhysicsField

An object that applies forces, such as gravitation, electromagnetism, and turbulence, to physics bodies within a certain area of effect.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class SCNPhysicsField
```

## Overview

You can create many types of field effects, such as gravitation, electromagnetism, and turbulence. To add a field effect to a scene, you create a physics field of the type you want to use and then attach it to the physicsField property of a node in the scene.

Physics fields can affect both SCNPhysicsBody objects and the particles spawned by SCNParticleSystem objects.

## Topics

### Creating Physics Fields

class func drag() -> SCNPhysicsField

Creates a field that slows any object in its area of effect with a force proportional to the object’s velocity.

class func vortex() -> SCNPhysicsField

Creates a field whose forces circulate around an axis.

class func radialGravity() -> SCNPhysicsField

Creates a field that accelerates objects toward its center.

class func linearGravity() -> SCNPhysicsField

Creates a field that accelerates objects in a specific direction.

class func noiseField(smoothness: CGFloat, animationSpeed: CGFloat) -> SCNPhysicsField

Creates a field that applies random forces to objects in its area of effect.

class func turbulenceField(smoothness: CGFloat, animationSpeed: CGFloat) -> SCNPhysicsField

Creates a field that applies random forces to objects in its area of effect, with magnitudes proportional to those objects’ velocities.

class func spring() -> SCNPhysicsField

Creates a field that pulls objects toward its center with a spring-like force.

class func electric() -> SCNPhysicsField

Creates a field that attracts or repels objects based on their electrical charge and on their distance from the field’s center.

class func magnetic() -> SCNPhysicsField

Creates a field that attracts or repels objects based on their electrical charge, velocity, and distance from the field’s axis.

### Creating Custom Physics Fields

class func customField(evaluationBlock: SCNFieldForceEvaluator) -> SCNPhysicsField

Creates a field that runs the specified block to determine the force a field applies to each object in its area of effect.

### Specifying a Field’s Area of Effect

var halfExtent: SCNVector3

A location marking the end of the field’s area of effect.

var scope: SCNPhysicsFieldScope

The area affected by the field, either inside or outside its region.

var usesEllipsoidalExtent: Bool

A Boolean value that determines whether the field’s area of effect is shaped like a box or ellipsoid.

var offset: SCNVector3

The offset of the field’s center within its area of effect.

var direction: SCNVector3

The field’s directional axis.

### Specifying a Field’s Behavior

var strength: CGFloat

A multiplier for the force that the field applies to objects in its area of effect.

var falloffExponent: CGFloat

An exponent that determines how the field’s strength diminishes with distance.

var minimumDistance: CGFloat

The minimum value for distance-based effects.

var isActive: Bool

A Boolean value that determines whether the field’s effect is enabled.

var isExclusive: Bool

A Boolean value that determines whether the field overrides other fields whose areas of effect it overlaps.

### Choosing Physics Bodies to Be Affected by the Field

var categoryBitMask: Int

A mask that defines which categories this physics field belongs to.

### Constants

typealias SCNFieldForceEvaluator

The signature for a block that SceneKit calls to determine the effect of a custom field on an object.

enum SCNPhysicsFieldScope

Options for defining the region of space affected by a physics field, used by the scope property.

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

### Physics in a Scene

class SCNPhysicsWorld

The global simulation of collisions, gravity, joints, and other physics effects in a scene.

class SCNPhysicsBehavior

The abstract superclass for joints, vehicle simulations, and other high-level behaviors that incorporate multiple physics bodies.

