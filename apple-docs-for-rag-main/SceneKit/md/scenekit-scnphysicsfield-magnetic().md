

- SceneKit
- SCNPhysicsField
-  magnetic() 

Type Method

# magnetic()

Creates a field that attracts or repels objects based on their electrical charge, velocity, and distance from the field’s axis.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class func magnetic() -> SCNPhysicsField
```

## Return Value

A physics field object. To use the field in a scene, attach it to the physicsField property of an SCNNode object.

## Discussion

Use this field type to make objects behave differently from one another when they enter a region, or to make an object’s behavior different from its mass based behavior. A magnetic field behaves according to the second part of the Lorentz force equation modeling real-world electromagnetic forces—the field applies a force determined by the cross product of an object’s velocity vector and the magnetic field vector at the object’s location, with magnitude proportional to the object’s electric charge.

By default, physics bodies and particle systems have no electric charge, so they are unaffected by electric and magnetic fields. Use the charge property of a physics body or the particleCharge property of a particle system to add charge-based behavior.

When the field’s strength value is positive (the default), the magnetic field vectors circulate counterclockwise relative to the field’s direction vector. (That is, the magnetic field models a real-world magnetic field created by current in a wire oriented in the field’s direction.) To make field vectors circulate clockwise, set the field’s strength property to a negative value.

Note

This SCNPhysicsField option models the real-world physics effect of magnetic fields on moving, electrically charged bodies, not the behavior of permanent magnets or electromagnets. To make objects in your scene simply attract or repel one another, use a different field type. For example, a field created by the radialGravity() method attracts or repels all dynamic bodies near it according to its strength property, and a field created by the electric() method selectively attracts or repels bodies according to their electric charge.

The default falloffExponent value for a magnetic field is `2.0`, indicating that the field’s effect diminishes with the square of distance from its center.

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

class func turbulenceField(smoothness: CGFloat, animationSpeed: CGFloat) -> SCNPhysicsField

Creates a field that applies random forces to objects in its area of effect, with magnitudes proportional to those objects’ velocities.

class func spring() -> SCNPhysicsField

Creates a field that pulls objects toward its center with a spring-like force.

class func electric() -> SCNPhysicsField

Creates a field that attracts or repels objects based on their electrical charge and on their distance from the field’s center.

