

- SceneKit
- SCNPhysicsField
-  linearGravity() 

Type Method

# linearGravity()

Creates a field that accelerates objects in a specific direction.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func linearGravity() -> SCNPhysicsField
```

## Return Value

A physics field object. To use the field in a scene, attach it to the physicsField property of an SCNNode object.

## Discussion

Because the force of gravity on an object is proportional to the object’s mass, this force accelerates all objects in the field’s area of affect by the same amount. The field’s strength property measures this acceleration in meters per second per second.

By default, a linear gravity field accelerates objects in along its direction vector. To make it accelerate objects in the opposite direction, set the field’s strength property to a negative value.

The default falloffExponent value for a linear gravity field is `0.0`, indicating that the field’s effect is constant throughout its area of effect.

## See Also

### Creating Physics Fields

class func drag() -> SCNPhysicsField

Creates a field that slows any object in its area of effect with a force proportional to the object’s velocity.

class func vortex() -> SCNPhysicsField

Creates a field whose forces circulate around an axis.

class func radialGravity() -> SCNPhysicsField

Creates a field that accelerates objects toward its center.

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

