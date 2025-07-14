

- SceneKit
- SCNPhysicsSliderJoint
-  motorTargetLinearVelocity 

Instance Property

# motorTargetLinearVelocity

The velocity at which the joint’s connected bodies should slide.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var motorTargetLinearVelocity: CGFloat { get set }
```

## Discussion

At the default value of `0.0`, the joint moves only when an external force acts on one of its connected bodies. Changing this value causes the joint to act as a linear motor, continuously applying a force (specified by the motorMaximumForce property) until its connected bodies are moving along the sliding axis of the joint at the new velocity.

## See Also

### Applying Forces and Torques

var motorMaximumForce: CGFloat

The maximum linear force that the joint can apply to its connected bodies, in newtons.

var motorTargetAngularVelocity: CGFloat

The angular velocity at which the joint’s connected bodies should rotate around it.

var motorMaximumTorque: CGFloat

The maximum torque that the joint can apply to its connected bodies, in newton-meters.

