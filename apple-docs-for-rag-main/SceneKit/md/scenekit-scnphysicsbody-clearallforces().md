

- SceneKit
- SCNPhysicsBody
-  clearAllForces() 

Instance Method

# clearAllForces()

Cancels all continuous forces and torques acting on the physics body during the current simulation step.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func clearAllForces()
```

## Discussion

When you pass false for the `impulse` parameter in the applyForce(_:asImpulse:), applyForce(_:at:asImpulse:), or applyTorque(_:asImpulse:) method, SceneKit waits until the end of the current simulation step before applying its effect. At that time, SceneKit sums all forces and torques applied during that simulation step and changes the velocity or angular velocity of the body according to the net effect of those forces and torques.

Call clearAllForces() to cancel any forces and torques previously applied during the current simulation step.

## See Also

### Applying Forces, Impulses, and Torques

func applyForce(SCNVector3, asImpulse: Bool)

Applies a force or impulse to the body at its center of mass.

func applyForce(SCNVector3, at: SCNVector3, asImpulse: Bool)

Applies a force or impulse to the body at a specific point.

func applyTorque(SCNVector4, asImpulse: Bool)

Applies a net torque or a change in angular momentum to the body.

