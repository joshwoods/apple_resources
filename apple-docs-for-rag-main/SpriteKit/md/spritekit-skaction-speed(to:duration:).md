

- SpriteKit
- SKAction
-  speed(to:duration:) 

Type Method

# speed(to:duration:)

Creates an action that changes how fast the node executes actions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func speed(
    to speed: CGFloat,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`speed`  

The new value for the node’s speed.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s speed property animates to the new value.

This action is not reversible; the reverse of this action has the same duration but does not change anything.

## See Also

### Controlling the Action’s Speed

class func speed(by: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that changes how fast the node executes actions by a relative value.

