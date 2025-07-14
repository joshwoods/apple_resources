

- SpriteKit
- SKPhysicsBody
-  applyTorque(\_:) 

Instance Method

# applyTorque(\_:)

Applies torque to an object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func applyTorque(_ torque: CGFloat)
```

## Parameters 

`torque`  

The amount of torque, in Newton-meters.

## Discussion

This method generates an angular acceleration on the body without causing any linear acceleration. The force is applied for a single simulation step (one frame).

## See Also

### Applying Forces and Impulses to a Physics Body

Making Physics Bodies Move

Move a body using various physics properties, like velocity, gravity or impulses.

func applyForce(CGVector)

Applies a force to the center of gravity of a physics body.

func applyForce(CGVector, at: CGPoint)

Applies a force to a specific point of a physics body.

func applyImpulse(CGVector)

Applies an impulse to the center of gravity of a physics body.

func applyAngularImpulse(CGFloat)

Applies an impulse that imparts angular momentum to an object.

func applyImpulse(CGVector, at: CGPoint)

Applies an impulse to a specific point of a physics body.

