

- SceneKit
- SCNPhysicsField
-  turbulenceField(smoothness:animationSpeed:) 

Type Method

# turbulenceField(smoothness:animationSpeed:)

Creates a field that applies random forces to objects in its area of effect, with magnitudes proportional to those objects’ velocities.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func turbulenceField(
    smoothness: CGFloat,
    animationSpeed speed: CGFloat
) -> SCNPhysicsField
```

## Parameters 

`smoothness`  

The amount of randomness in the field. A value of `0.0` specifies maximum noise, and a value of `1.0` specifies no noise at all.

`speed`  

The field’s variation over time. Specify `0.0` for a static field.

## Return Value

A physics field object. To use the field in a scene, attach it to the physicsField property of an SCNNode object.

## Discussion

Like a noise field, a turbulence field applies forces in random directions to the objects that it affects. Unlike a noise field, a turbulence field applies a force whose magnitude is proportional to the speed of each affected object. For example, an object passing through a noise field shakes as it travels through the field, but an object passing through a turbulence field shakes more violently the faster it travels. The field’s strength property scales the magnitude of the turbulence effect.

The default falloffExponent value for a turbulence field is `0.0`, indicating that the field’s effect is constant throughout its area of effect.

## See Also

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

class func spring() -> SCNPhysicsField

Creates a field that pulls objects toward its center with a spring-like force.

class func electric() -> SCNPhysicsField

Creates a field that attracts or repels objects based on their electrical charge and on their distance from the field’s center.

class func magnetic() -> SCNPhysicsField

Creates a field that attracts or repels objects based on their electrical charge, velocity, and distance from the field’s axis.

