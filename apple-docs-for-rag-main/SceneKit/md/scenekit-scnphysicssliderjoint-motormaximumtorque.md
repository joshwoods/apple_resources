

- SceneKit
- SCNPhysicsSliderJoint
-  motorMaximumTorque 

Instance Property

# motorMaximumTorque

The maximum torque that the joint can apply to its connected bodies, in newton-meters.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var motorMaximumTorque: CGFloat { get set }
```

## Discussion

When you change the value of the motorTargetAngularVelocity property, the joint continuously applies a force of no greater than this magnitude until the bodies are rotating around the joint at the target angular velocity. The default value is `1.0`.

## See Also

### Applying Forces and Torques

var motorTargetLinearVelocity: CGFloat

The velocity at which the joint’s connected bodies should slide.

var motorMaximumForce: CGFloat

The maximum linear force that the joint can apply to its connected bodies, in newtons.

var motorTargetAngularVelocity: CGFloat

The angular velocity at which the joint’s connected bodies should rotate around it.

