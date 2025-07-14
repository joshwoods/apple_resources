

- SceneKit
- SCNPhysicsField
-  noiseField(smoothness:animationSpeed:) 

Type Method

# noiseField(smoothness:animationSpeed:)

Creates a field that applies random forces to objects in its area of effect.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func noiseField(
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

Use this field type to simulate effects involving random motion, such as fireflies or gently falling snow.

In calculating the direction and strength of the field’s effect on an object, SceneKit uses a Perlin simplex noise function. This function produces a velocity field that varies over time.

The default falloffExponent value for a noise field is `0.0`, indicating that the field’s effect is constant throughout its area of effect. This field type ignores the field’s direction property.

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

class func turbulenceField(smoothness: CGFloat, animationSpeed: CGFloat) -> SCNPhysicsField

Creates a field that applies random forces to objects in its area of effect, with magnitudes proportional to those objects’ velocities.

class func spring() -> SCNPhysicsField

Creates a field that pulls objects toward its center with a spring-like force.

class func electric() -> SCNPhysicsField

Creates a field that attracts or repels objects based on their electrical charge and on their distance from the field’s center.

class func magnetic() -> SCNPhysicsField

Creates a field that attracts or repels objects based on their electrical charge, velocity, and distance from the field’s axis.

