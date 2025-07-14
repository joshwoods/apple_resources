

- SpriteKit
- SKPhysicsBody
-  applyAngularImpulse(\_:) 

Instance Method

# applyAngularImpulse(\_:)

Applies an impulse that imparts angular momentum to an object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func applyAngularImpulse(_ impulse: CGFloat)
```

## Parameters 

`impulse`  

The magnitude of the impulse. The impulse is measured in Newton-seconds.

## Discussion

This method affects the body’s angular velocity without changing the body’s linear velocity.

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

func applyImpulse(CGVector)

Applies an impulse to the center of gravity of a physics body.

func applyImpulse(CGVector, at: CGPoint)

Applies an impulse to a specific point of a physics body.

