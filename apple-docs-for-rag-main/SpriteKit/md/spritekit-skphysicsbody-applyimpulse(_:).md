

- SpriteKit
- SKPhysicsBody
-  applyImpulse(\_:) 

Instance Method

# applyImpulse(\_:)

Applies an impulse to the center of gravity of a physics body.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func applyImpulse(_ impulse: CGVector)
```

## Parameters 

`impulse`  

A vector that describes how much momentum was imparted in each dimension. The impulse is measured in Newton-seconds.

## Discussion

This method affects the body’s linear velocity without changing the body’s angular velocity.

## See Also

### Applying Forces and Impulses to a Physics Body

Making Physics Bodies Move

Move a body using various physics properties, like velocity, gravity or impulses.

func applyForce(CGVector)

Applies a force to the center of gravity of a physics body.

func applyTorque(CGFloat)

Applies torque to an object.

func applyForce(CGVector, at: CGPoint)

Applies a force to a specific point of a physics body.

func applyAngularImpulse(CGFloat)

Applies an impulse that imparts angular momentum to an object.

func applyImpulse(CGVector, at: CGPoint)

Applies an impulse to a specific point of a physics body.

