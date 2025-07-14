

- SceneKit
- SCNPhysicsSliderJoint
-  motorTargetAngularVelocity 

Instance Property

# motorTargetAngularVelocity

The angular velocity at which the joint’s connected bodies should rotate around it.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var motorTargetAngularVelocity: CGFloat { get set }
```

## Discussion

At the default value of `0.0`, the joint moves only when an external force acts on one of its connected bodies. Changing this value causes the joint to act as a rotary motor, continuously applying a torque (specified by the motorMaximumTorque property) until its connected bodies are rotating around the joint at the new angular velocity.

## See Also

### Applying Forces and Torques

var motorTargetLinearVelocity: CGFloat

The velocity at which the joint’s connected bodies should slide.

var motorMaximumForce: CGFloat

The maximum linear force that the joint can apply to its connected bodies, in newtons.

var motorMaximumTorque: CGFloat

The maximum torque that the joint can apply to its connected bodies, in newton-meters.

