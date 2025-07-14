

- SpriteKit
- SKPhysicsBody
-  applyForce(\_:) 

Instance Method

# applyForce(\_:)

Applies a force to the center of gravity of a physics body.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func applyForce(_ force: CGVector)
```

## Parameters 

`force`  

A vector that describes how much force was applied in each dimension. The force is measured in Newtons.

## Discussion

This method accelerates the body without imparting any angular acceleration to it. The acceleration is applied for a single simulation step (one frame).

## See Also

### Applying Forces and Impulses to a Physics Body

Making Physics Bodies Move

Move a body using various physics properties, like velocity, gravity or impulses.

func applyTorque(CGFloat)

Applies torque to an object.

func applyForce(CGVector, at: CGPoint)

Applies a force to a specific point of a physics body.

func applyImpulse(CGVector)

Applies an impulse to the center of gravity of a physics body.

func applyAngularImpulse(CGFloat)

Applies an impulse that imparts angular momentum to an object.

func applyImpulse(CGVector, at: CGPoint)

Applies an impulse to a specific point of a physics body.

