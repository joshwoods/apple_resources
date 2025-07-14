

- SpriteKit
- SKPhysicsBody
-  applyForce(\_:at:) 

Instance Method

# applyForce(\_:at:)

Applies a force to a specific point of a physics body.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func applyForce(
    _ force: CGVector,
    at point: CGPoint
)
```

## Parameters 

`force`  

A vector that describes how much force was applied in each dimension. The force is measured in Newtons.

`point`  

A point in scene coordinates that defines where the force was applied to the physics body.

## Discussion

Because the force is applied to a specific point on the body, it may impart both linear acceleration and angular acceleration. The force is applied for a single simulation step (one frame).

## See Also

### Applying Forces and Impulses to a Physics Body

Making Physics Bodies Move

Move a body using various physics properties, like velocity, gravity or impulses.

func applyForce(CGVector)

Applies a force to the center of gravity of a physics body.

func applyTorque(CGFloat)

Applies torque to an object.

func applyImpulse(CGVector)

Applies an impulse to the center of gravity of a physics body.

func applyAngularImpulse(CGFloat)

Applies an impulse that imparts angular momentum to an object.

func applyImpulse(CGVector, at: CGPoint)

Applies an impulse to a specific point of a physics body.

