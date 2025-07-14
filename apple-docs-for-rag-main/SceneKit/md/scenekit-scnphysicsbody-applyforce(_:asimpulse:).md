

- SceneKit
- SCNPhysicsBody
-  applyForce(\_:asImpulse:) 

Instance Method

# applyForce(\_:asImpulse:)

Applies a force or impulse to the body at its center of mass.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func applyForce(
    _ direction: SCNVector3,
    asImpulse impulse: Bool
)
```

## Parameters 

`direction`  

The direction and magnitude of the force (in newtons) or of the impulse (in newton-seconds).

`impulse`  

true to apply an instantaneous change in momentum; false to apply a force that affects the body at the end of the simulation step.

## Discussion

Applying a force or impulse to a body imparts a linear acceleration proportional to its mass.

The `impulse` parameter determines how this method contributes to the physics simulation:

- If you specify true, SceneKit treats the `direction` parameter as an impulse, measured in newton-seconds, and accelerates the physics body immediately. Use this option to simulate instantaneous effects such as launching a projectile.

- If you specify false, SceneKit treats the `direction` parameter as a force, measured in newtons. At the end of each simulation step (by default, a step occurs once for each frame in the rendering loop), SceneKit sums all forces applied to the physics body during that step and accelerates the body according to the net effect of those forces. Use this option when you want to simulate continuous forces on the body by calling applyForce(_:asImpulse:) on each simulation step.

Note

The `impulse` parameter effectively changes the unit of magnitude. A value that results in a certain acceleration when applied continuously on each frame of the simulation results in much less acceleration if applied only during a single frame.

As with all physical quantities in SceneKit, you need not use realistic force measurements in your app—the effects of the physics simulation depend on the relative differences between forces, not on their absolute values. You may use whatever values produce the behavior or gameplay you’re looking for as long as you use them consistently.

## See Also

### Applying Forces, Impulses, and Torques

func applyForce(SCNVector3, at: SCNVector3, asImpulse: Bool)

Applies a force or impulse to the body at a specific point.

func applyTorque(SCNVector4, asImpulse: Bool)

Applies a net torque or a change in angular momentum to the body.

func clearAllForces()

Cancels all continuous forces and torques acting on the physics body during the current simulation step.

