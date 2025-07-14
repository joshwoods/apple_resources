

- SceneKit
- SCNPhysicsField
-  drag() 

Type Method

# drag()

Creates a field that slows any object in its area of effect with a force proportional to the object’s velocity.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func drag() -> SCNPhysicsField
```

## Return Value

A physics field object. To use the field in a scene, attach it to the physicsField property of an SCNNode object.

## Discussion

Like the damping and angularDamping properties of a physics body, drag fields can simulate effects such as fluid friction or air resistance. Unlike those properties, drag fields can simulate different intensities of fluid friction in different areas of your scene. For example, you can use a drag field to represent underwater areas.

The default falloffExponent value for a drag field is `0.0`, indicating that the field’s effect is constant throughout its area of effect.

## See Also

### Creating Physics Fields

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

