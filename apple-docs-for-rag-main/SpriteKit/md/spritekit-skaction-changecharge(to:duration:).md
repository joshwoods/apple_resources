

- SpriteKit
- SKAction
-  changeCharge(to:duration:) 

Type Method

# changeCharge(to:duration:)

Creates an action that changes the charge of a node’s physics body to a new value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func changeCharge(
    to v: Float,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`v`  

The new charge of the physics body.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the physics body’s charge property animates from its current value to its new value.

This action is not reversible.

## See Also

### Animating Properties of a Node’s Physics Body

class func applyForce(CGVector, duration: TimeInterval) -> SKAction

Creates an action that applies a force to the center of gravity of a node’s physics body.

class func applyTorque(CGFloat, duration: TimeInterval) -> SKAction

Creates an action that applies a torque to a node’s physics body.

class func applyForce(CGVector, at: CGPoint, duration: TimeInterval) -> SKAction

Creates an action that applies a force to a specific point on a node’s physics body.

class func applyImpulse(CGVector, duration: TimeInterval) -> SKAction

Creates an action that applies an impulse to the center of gravity of a physics body.

class func applyAngularImpulse(CGFloat, duration: TimeInterval) -> SKAction

Creates an action that applies an angular impulse to a node’s physics body.

class func applyImpulse(CGVector, at: CGPoint, duration: TimeInterval) -> SKAction

Creates an action that applies an impulse to a specific point of a node’s physics body.

class func applyImpulse(CGVector, duration: TimeInterval) -> SKAction

Creates an action that applies an impulse to the center of gravity of a physics body.

class func changeCharge(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes the charge of a node’s physics body by a relative value.

class func changeMass(to: Float, duration: TimeInterval) -> SKAction

Creates an action that changes the mass of a node’s physics body to a new value.

class func changeMass(by: Float, duration: TimeInterval) -> SKAction

Creates an action that changes the mass of a node’s physics body by a relative value.

class func strength(to: Float, duration: TimeInterval) -> SKAction

Creates an action that animates a change of a physics field’s strength.

class func strength(by: Float, duration: TimeInterval) -> SKAction

Creates an action that animates a change of a physics field’s strength to a value relative to the existing value.

class func falloff(to: Float, duration: TimeInterval) -> SKAction

Creates an action that animates a change of a physics field’s falloff.

class func falloff(by: Float, duration: TimeInterval) -> SKAction

Creates an action that animates a change of a physics field’s falloff to a value relative to the existing value.

