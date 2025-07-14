

- SpriteKit
- SKAction
-  fadeAlpha(to:duration:) 

Type Method

# fadeAlpha(to:duration:)

Creates an action that adjusts the alpha value of a node to a new value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func fadeAlpha(
    to alpha: CGFloat,
    duration: TimeInterval
) -> SKAction
```

## Parameters 

`alpha`  

The new value of the node’s alpha.

`duration`  

The duration of the animation.

## Return Value

A new action object.

## Discussion

When the action executes, the node’s alpha property animates to its new value.

This action is not reversible; the reverse of this action has the same duration but does not change anything.

## See Also

### Animating the Transparency of a Node

class func fadeIn(withDuration: TimeInterval) -> SKAction

Creates an action that changes the alpha value of the node to `1.0`.

class func fadeOut(withDuration: TimeInterval) -> SKAction

Creates an action that changes the alpha value of the node to `0.0`.

class func fadeAlpha(by: CGFloat, duration: TimeInterval) -> SKAction

Creates an action that adjusts the alpha value of a node by a relative value.

