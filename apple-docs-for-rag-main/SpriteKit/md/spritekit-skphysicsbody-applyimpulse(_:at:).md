

- SpriteKit
- SKPhysicsBody
-  applyImpulse(\_:at:) 

Instance Method

# applyImpulse(\_:at:)

Applies an impulse to a specific point of a physics body.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func applyImpulse(
    _ impulse: CGVector,
    at point: CGPoint
)
```

## Parameters 

`impulse`  

A vector that describes how much momentum to impart to the body. The impulse is measured in Newton-seconds.

`point`  

A point in scene coordinates that defines where the impulse was applied to the physics body.

## Discussion

Because this impulse is applied to a specific point on the object, it may change both the body’s velocity and angular velocity.

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

func applyAngularImpulse(CGFloat)

Applies an impulse that imparts angular momentum to an object.

