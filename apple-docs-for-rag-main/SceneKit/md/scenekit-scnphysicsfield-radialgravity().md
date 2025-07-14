

- SceneKit
- SCNPhysicsField
-  radialGravity() 

Type Method

# radialGravity()

Creates a field that accelerates objects toward its center.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func radialGravity() -> SCNPhysicsField
```

## Return Value

A physics field object. To use the field in a scene, attach it to the physicsField property of an SCNNode object.

## Discussion

Because the force of gravity on an object is proportional to the object’s mass, this force accelerates all objects at the same distance from the field’s center by the same amount. The field’s strength property measures this acceleration in meters per second per second.

By default, a radial gravity field attracts objects toward its center. To make it repel objects instead, set the field’s strength property to a negative value.

The default falloffExponent value for a radial gravity field is `2.0`, indicating that the field’s effect diminishes with the square of distance from its center.

## See Also

### Creating Physics Fields

class func drag() -> SCNPhysicsField

Creates a field that slows any object in its area of effect with a force proportional to the object’s velocity.

class func vortex() -> SCNPhysicsField

Creates a field whose forces circulate around an axis.

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

